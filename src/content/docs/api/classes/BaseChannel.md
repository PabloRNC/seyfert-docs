---
editUrl: false
next: false
prev: false
title: "BaseChannel"
---

## Extends

- `DiscordBase`\<`APIChannelBase`\<`ChannelType`\>\>

## Type parameters

| Type parameter |
| :------ |
| `T` extends `ChannelType` |

## Constructors

### new BaseChannel(client, data)

```ts
new BaseChannel<T>(client: BaseClient, data: APIChannelBase<ChannelType>): BaseChannel<T>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `client` | `BaseClient` |
| `data` | `APIChannelBase`\<`ChannelType`\> |

#### Returns

[`BaseChannel`](/api/classes/basechannel/)\<`T`\>

#### Overrides

`DiscordBase<APIChannelBase<ChannelType>>.constructor`

#### Source

[seyfert/src/structures/channels.ts:48](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L48)

## Properties

| Property | Modifier | Type | Inherited from |
| :------ | :------ | :------ | :------ |
| `client` | `readonly` | [`UsingClient`](/api/interfaces/usingclient/) | `DiscordBase.client` |
| `id` | `public` | `string` | `DiscordBase.id` |
| `type` | `public` | `T` | - |

## Accessors

### createdAt

```ts
get createdAt(): Date
```

createdAt gets the creation Date instace of the current object.

#### Returns

`Date`

#### Source

[seyfert/src/structures/extra/DiscordBase.ts:27](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/extra/DiscordBase.ts#L27)

***

### createdTimestamp

```ts
get createdTimestamp(): number
```

Create a timestamp for the current object.

#### Returns

`number`

#### Source

[seyfert/src/structures/extra/DiscordBase.ts:20](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/extra/DiscordBase.ts#L20)

***

### url

```ts
get url(): string
```

The URL to the channel

#### Returns

`string`

#### Source

[seyfert/src/structures/channels.ts:59](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L59)

## Methods

### delete()

```ts
delete(reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Source

[seyfert/src/structures/channels.ts:67](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L67)

***

### edit()

```ts
edit(body: RESTPatchAPIChannelJSONBody, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `RESTPatchAPIChannelJSONBody` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Source

[seyfert/src/structures/channels.ts:71](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L71)

***

### fetch()

```ts
fetch(force: boolean): Promise<AllChannels>
```

#### Parameters

| Parameter | Type | Default value |
| :------ | :------ | :------ |
| `force` | `boolean` | `false` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Source

[seyfert/src/structures/channels.ts:63](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L63)

***

### is()

```ts
is<T>(channelTypes: T): this is IChannelTypes[T[number]]
```

#### Type parameters

| Type parameter |
| :------ |
| `T` extends keyof `IChannelTypes`[] |

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `channelTypes` | `T` |

#### Returns

`this is IChannelTypes[T[number]]`

#### Source

[seyfert/src/structures/channels.ts:131](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L131)

***

### isCategory()

```ts
isCategory(): this is CategoryChannel
```

#### Returns

`this is CategoryChannel`

#### Source

[seyfert/src/structures/channels.ts:111](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L111)

***

### isDM()

```ts
isDM(): this is DMChannel
```

#### Returns

`this is DMChannel`

#### Source

[seyfert/src/structures/channels.ts:87](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L87)

***

### isDirectory()

```ts
isDirectory(): this is DirectoryChannel
```

#### Returns

`this is DirectoryChannel`

#### Source

[seyfert/src/structures/channels.ts:99](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L99)

***

### isForum()

```ts
isForum(): this is ForumChannel
```

#### Returns

`this is ForumChannel`

#### Source

[seyfert/src/structures/channels.ts:91](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L91)

***

### isGuildTextable()

```ts
isGuildTextable(): this is AllGuildTextableChannels
```

#### Returns

`this is AllGuildTextableChannels`

#### Source

[seyfert/src/structures/channels.ts:123](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L123)

***

### isMedia()

```ts
isMedia(): this is MediaChannel
```

#### Returns

`this is MediaChannel`

#### Source

[seyfert/src/structures/channels.ts:83](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L83)

***

### isNews()

```ts
isNews(): this is NewsChannel
```

#### Returns

`this is NewsChannel`

#### Source

[seyfert/src/structures/channels.ts:115](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L115)

***

### isStage()

```ts
isStage(): this is StageChannel
```

#### Returns

`this is StageChannel`

#### Source

[seyfert/src/structures/channels.ts:79](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L79)

***

### isTextGuild()

```ts
isTextGuild(): this is TextGuildChannel
```

#### Returns

`this is TextGuildChannel`

#### Source

[seyfert/src/structures/channels.ts:107](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L107)

***

### isTextable()

```ts
isTextable(): this is AllTextableChannels
```

#### Returns

`this is AllTextableChannels`

#### Source

[seyfert/src/structures/channels.ts:119](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L119)

***

### isThread()

```ts
isThread(): this is ThreadChannel
```

#### Returns

`this is ThreadChannel`

#### Source

[seyfert/src/structures/channels.ts:95](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L95)

***

### isThreadOnly()

```ts
isThreadOnly(): this is MediaChannel | ForumChannel
```

#### Returns

`this is MediaChannel | ForumChannel`

#### Source

[seyfert/src/structures/channels.ts:127](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L127)

***

### isVoice()

```ts
isVoice(): this is VoiceChannel
```

#### Returns

`this is VoiceChannel`

#### Source

[seyfert/src/structures/channels.ts:103](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L103)

***

### toString()

```ts
toString(): string
```

#### Returns

`string`

#### Source

[seyfert/src/structures/channels.ts:75](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L75)

***

### \_\_intent\_\_()

#### \_\_intent\_\_(id)

```ts
static __intent__(id: "@me"): "DirectMessages"
```

##### Parameters

| Parameter | Type |
| :------ | :------ |
| `id` | `"@me"` |

##### Returns

`"DirectMessages"`

##### Source

[seyfert/src/structures/channels.ts:52](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L52)

#### \_\_intent\_\_(id)

```ts
static __intent__(id: string): "Guilds" | "DirectMessages"
```

##### Parameters

| Parameter | Type |
| :------ | :------ |
| `id` | `string` |

##### Returns

`"Guilds"` \| `"DirectMessages"`

##### Source

[seyfert/src/structures/channels.ts:53](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L53)

***

### allMethods()

```ts
static allMethods(ctx:     Object): Object
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `ctx` | `Object` |
| `ctx.client` | `BaseClient` |
| `ctx.guildId` | `string` |

#### Returns

`Object`

| Member | Type | Value |
| :------ | :------ | :------ |
| `create` | (`body`: `RESTPostAPIGuildChannelJSONBody`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `delete` | (`id`: `string`, `reason`?: `string`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `edit` | (`id`: `string`, `body`: `RESTPatchAPIChannelJSONBody`, `reason`?: `string`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `editPositions` | (`body`: `RESTPatchAPIGuildChannelPositionsJSONBody`) => `Promise`\<`never`\> | - |
| `fetch` | (`id`: `string`, `force`: `boolean`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `list` | (`force`: `boolean`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)[]\> | - |

#### Source

[seyfert/src/structures/channels.ts:135](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L135)