---
editUrl: false
next: false
prev: false
title: "StageChannel"
---

## Extends

- `ObjectToLower`\<`Omit`\<`APIGuildStageVoiceChannel`, `"type"`\>\>.[`TopicableGuildChannel`](/api/classes/topicableguildchannel/).[`VoiceChannelMethods`](/api/classes/voicechannelmethods/).[`BaseChannel`](/api/classes/basechannel/)\<`ChannelType`\>

## Constructors

### new StageChannel(client, data)

```ts
new StageChannel(client: BaseClient, data: APIChannelBase<ChannelType>): StageChannel
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `client` | `BaseClient` |
| `data` | `APIChannelBase`\<`ChannelType`\> |

#### Returns

[`StageChannel`](/api/classes/stagechannel/)

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`constructor`](/api/classes/basechannel/#constructors)

#### Source

[seyfert/src/structures/channels.ts:48](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L48)

## Properties

| Property | Modifier | Type | Inherited from |
| :------ | :------ | :------ | :------ |
| `bitrate` | `public` | `undefined` \| `number` | `ObjectToLower.bitrate` |
| `client` | `readonly` | [`UsingClient`](/api/interfaces/usingclient/) | [`BaseChannel`](/api/classes/basechannel/).`client` |
| `flags` | `public` | `undefined` \| `ChannelFlags` | `ObjectToLower.flags` |
| `guildId` | `public` | `undefined` \| `string` | `ObjectToLower.guildId` |
| `id` | `public` | `string` | [`BaseChannel`](/api/classes/basechannel/).`id` |
| `lastMessageId` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.lastMessageId` |
| `name` | `public` | `string` | `ObjectToLower.name` |
| `nsfw` | `public` | `undefined` \| `boolean` | `ObjectToLower.nsfw` |
| `parentId` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.parentId` |
| `permissionOverwrites` | `public` | `undefined` \| `APIOverwrite`[] | `ObjectToLower.permissionOverwrites` |
| `position` | `public` | `number` | `ObjectToLower.position` |
| `rateLimitPerUser` | `public` | `undefined` \| `number` | `ObjectToLower.rateLimitPerUser` |
| `rtcRegion` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.rtcRegion` |
| `type` | `public` | `GuildStageVoice` | [`BaseChannel`](/api/classes/basechannel/).`type` |
| `userLimit` | `public` | `undefined` \| `number` | `ObjectToLower.userLimit` |
| `videoQualityMode` | `public` | `undefined` \| `VideoQualityMode` | `ObjectToLower.videoQualityMode` |

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

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`delete`](/api/classes/basechannel/#delete)

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

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`edit`](/api/classes/basechannel/#edit)

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

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`fetch`](/api/classes/basechannel/#fetch)

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

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`is`](/api/classes/basechannel/#is)

#### Source

[seyfert/src/structures/channels.ts:131](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L131)

***

### isCategory()

```ts
isCategory(): this is CategoryChannel
```

#### Returns

`this is CategoryChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isCategory`](/api/classes/basechannel/#iscategory)

#### Source

[seyfert/src/structures/channels.ts:111](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L111)

***

### isDM()

```ts
isDM(): this is DMChannel
```

#### Returns

`this is DMChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isDM`](/api/classes/basechannel/#isdm)

#### Source

[seyfert/src/structures/channels.ts:87](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L87)

***

### isDirectory()

```ts
isDirectory(): this is DirectoryChannel
```

#### Returns

`this is DirectoryChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isDirectory`](/api/classes/basechannel/#isdirectory)

#### Source

[seyfert/src/structures/channels.ts:99](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L99)

***

### isForum()

```ts
isForum(): this is ForumChannel
```

#### Returns

`this is ForumChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isForum`](/api/classes/basechannel/#isforum)

#### Source

[seyfert/src/structures/channels.ts:91](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L91)

***

### isGuildTextable()

```ts
isGuildTextable(): this is AllGuildTextableChannels
```

#### Returns

`this is AllGuildTextableChannels`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isGuildTextable`](/api/classes/basechannel/#isguildtextable)

#### Source

[seyfert/src/structures/channels.ts:123](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L123)

***

### isMedia()

```ts
isMedia(): this is MediaChannel
```

#### Returns

`this is MediaChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isMedia`](/api/classes/basechannel/#ismedia)

#### Source

[seyfert/src/structures/channels.ts:83](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L83)

***

### isNews()

```ts
isNews(): this is NewsChannel
```

#### Returns

`this is NewsChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isNews`](/api/classes/basechannel/#isnews)

#### Source

[seyfert/src/structures/channels.ts:115](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L115)

***

### isStage()

```ts
isStage(): this is StageChannel
```

#### Returns

`this is StageChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isStage`](/api/classes/basechannel/#isstage)

#### Source

[seyfert/src/structures/channels.ts:79](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L79)

***

### isTextGuild()

```ts
isTextGuild(): this is TextGuildChannel
```

#### Returns

`this is TextGuildChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isTextGuild`](/api/classes/basechannel/#istextguild)

#### Source

[seyfert/src/structures/channels.ts:107](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L107)

***

### isTextable()

```ts
isTextable(): this is AllTextableChannels
```

#### Returns

`this is AllTextableChannels`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isTextable`](/api/classes/basechannel/#istextable)

#### Source

[seyfert/src/structures/channels.ts:119](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L119)

***

### isThread()

```ts
isThread(): this is ThreadChannel
```

#### Returns

`this is ThreadChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isThread`](/api/classes/basechannel/#isthread)

#### Source

[seyfert/src/structures/channels.ts:95](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L95)

***

### isThreadOnly()

```ts
isThreadOnly(): this is MediaChannel | ForumChannel
```

#### Returns

`this is MediaChannel | ForumChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isThreadOnly`](/api/classes/basechannel/#isthreadonly)

#### Source

[seyfert/src/structures/channels.ts:127](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L127)

***

### isVoice()

```ts
isVoice(): this is VoiceChannel
```

#### Returns

`this is VoiceChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isVoice`](/api/classes/basechannel/#isvoice)

#### Source

[seyfert/src/structures/channels.ts:103](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L103)

***

### setBitrate()

```ts
setBitrate(bitrate: null | number, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `bitrate` | `null` \| `number` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`VoiceChannelMethods`](/api/classes/voicechannelmethods/).[`setBitrate`](/api/classes/voicechannelmethods/#setbitrate)

#### Source

[seyfert/src/structures/channels.ts:335](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L335)

***

### setRTC()

```ts
setRTC(rtc_region: null | string, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `rtc_region` | `null` \| `string` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`VoiceChannelMethods`](/api/classes/voicechannelmethods/).[`setRTC`](/api/classes/voicechannelmethods/#setrtc)

#### Source

[seyfert/src/structures/channels.ts:343](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L343)

***

### setTopic()

```ts
setTopic(topic: null | string, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `topic` | `null` \| `string` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`TopicableGuildChannel`](/api/classes/topicableguildchannel/).[`setTopic`](/api/classes/topicableguildchannel/#settopic)

#### Source

[seyfert/src/structures/channels.ts:304](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L304)

***

### setUserLimit()

```ts
setUserLimit(user_limit: null | number, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `user_limit` | `null` \| `number` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`VoiceChannelMethods`](/api/classes/voicechannelmethods/).[`setUserLimit`](/api/classes/voicechannelmethods/#setuserlimit)

#### Source

[seyfert/src/structures/channels.ts:339](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L339)

***

### setVideoQuality()

```ts
setVideoQuality(quality: "Auto" | "Full", reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `quality` | `"Auto"` \| `"Full"` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`VoiceChannelMethods`](/api/classes/voicechannelmethods/).[`setVideoQuality`](/api/classes/voicechannelmethods/#setvideoquality)

#### Source

[seyfert/src/structures/channels.ts:347](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L347)

***

### toString()

```ts
toString(): string
```

#### Returns

`string`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`toString`](/api/classes/basechannel/#tostring)

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

##### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`__intent__`](/api/classes/basechannel/#__intent__)

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

##### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`__intent__`](/api/classes/basechannel/#__intent__)

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

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`allMethods`](/api/classes/basechannel/#allmethods)

#### Source

[seyfert/src/structures/channels.ts:135](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L135)