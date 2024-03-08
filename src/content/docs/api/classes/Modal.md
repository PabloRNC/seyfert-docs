---
editUrl: false
next: false
prev: false
title: "Modal"
---

Represents a modal for user interactions.

## Example

```ts
const modal = new Modal();
modal.setTitle("Sample Modal");
modal.addComponents(new TextInput().setLabel("Enter text"));
modal.run((interaction) => {
  // Handle modal submission
});
const json = modal.toJSON();
```

## Type parameters

| Type parameter | Value | Description |
| :------ | :------ | :------ |
| `T` extends [`ModalBuilderComponents`](/api/type-aliases/modalbuildercomponents/) | [`TextInput`](/api/classes/textinput/) | The type of components allowed in the modal. |

## Constructors

### new Modal(data)

```ts
new Modal<T>(data: Partial<APIModalInteractionResponseCallbackData>): Modal<T>
```

Creates a new Modal instance.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `data` | `Partial`\<`APIModalInteractionResponseCallbackData`\> | Optional data for the modal. |

#### Returns

[`Modal`](/api/classes/modal/)\<`T`\>

#### Source

[seyfert/src/builders/Modal.ts:35](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L35)

## Properties

| Property | Modifier | Type | Description |
| :------ | :------ | :------ | :------ |
| `components` | `public` | [`ActionRow`](/api/classes/actionrow/)\<`T`\>[] | - |
| `data` | `public` | `Partial`\<`APIModalInteractionResponseCallbackData`\> | Optional data for the modal. |

## Methods

### addComponents()

```ts
addComponents(...components: RestOrArray<ActionRow<T>>): this
```

Adds components to the modal.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| ...`components` | `RestOrArray`\<[`ActionRow`](/api/classes/actionrow/)\<`T`\>\> | Components to be added to the modal. |

#### Returns

`this`

The current Modal instance.

#### Source

[seyfert/src/builders/Modal.ts:44](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L44)

***

### run()

```ts
run(func: ModalSubmitCallback): this
```

Sets the callback function to be executed when the modal is submitted.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `func` | [`ModalSubmitCallback`](/api/type-aliases/modalsubmitcallback/) | The callback function. |

#### Returns

`this`

The current Modal instance.

#### Source

[seyfert/src/builders/Modal.ts:74](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L74)

***

### setCustomId()

```ts
setCustomId(id: string): this
```

Sets the custom ID of the modal.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `id` | `string` | The custom ID for the modal. |

#### Returns

`this`

The current Modal instance.

#### Source

[seyfert/src/builders/Modal.ts:64](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L64)

***

### setTitle()

```ts
setTitle(title: string): this
```

Sets the title of the modal.

#### Parameters

| Parameter | Type | Description |
| :------ | :------ | :------ |
| `title` | `string` | The title of the modal. |

#### Returns

`this`

The current Modal instance.

#### Source

[seyfert/src/builders/Modal.ts:54](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L54)

***

### toJSON()

```ts
toJSON(): APIModalInteractionResponseCallbackData
```

Converts the modal to JSON format.

#### Returns

`APIModalInteractionResponseCallbackData`

The modal data in JSON format.

#### Source

[seyfert/src/builders/Modal.ts:83](https://github.com/potoland/potocuit/blob/c4fb0c1/src/builders/Modal.ts#L83)