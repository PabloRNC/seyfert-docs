---
editUrl: false
next: false
prev: false
title: "WebhookChannelMethods"
---

## Extends

- `DiscordBase`

## Constructors

### new WebhookChannelMethods(client, data)

```ts
new WebhookChannelMethods(client: BaseClient, data:     Object): WebhookChannelMethods
```

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `client` | `BaseClient` | - |
| `data` | `Object` | Unique ID of the object |
| `data.id` | `string` | - |

#### Returns

[`WebhookChannelMethods`](/api/classes/webhookchannelmethods/)

#### Inherited from

`DiscordBase.constructor`

#### Source

[seyfert/src/structures/extra/DiscordBase.ts:7](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/extra/DiscordBase.ts#L7)

## Properties

| Property | Modifier | Type | Inherited from |
| :------ | :------ | :------ | :------ |
| `client` | `readonly` | [`UsingClient`](/api/interfaces/usingclient/) | `DiscordBase.client` |
| `id` | `public` | `string` | `DiscordBase.id` |
| `webhooks` | `public` | `Object` | - |
| `webhooks.create` | `public` | (`body`: `RESTPostAPIChannelWebhookJSONBody`) => `Promise`\<[`Webhook`](/api/classes/webhook/)\> | - |
| `webhooks.list` | `public` | () => `Promise`\<[`Webhook`](/api/classes/webhook/)[]\> | - |

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

## Methods

### channel()

```ts
static channel(ctx:     Object): Object
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `ctx` | `Object` |
| `ctx.channelId` | `string` |
| `ctx.client` | `BaseClient` |

#### Returns

`Object`

| Member | Type | Value |
| :------ | :------ | :------ |
| `create` | (`body`: `RESTPostAPIChannelWebhookJSONBody`) => `Promise`\<[`Webhook`](/api/classes/webhook/)\> | - |
| `list` | () => `Promise`\<[`Webhook`](/api/classes/webhook/)[]\> | - |

#### Source

[seyfert/src/structures/channels.ts:368](https://github.com/potoland/potocuit/blob/c4fb0c1/src/structures/channels.ts#L368)