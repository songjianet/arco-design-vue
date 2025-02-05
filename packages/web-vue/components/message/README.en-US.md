```yaml
meta:
  type: Component
  category: Feedback
title: Message
description: Lightweight global feedback triggered by user actions.
```

*Auto translate by google.*

@import ./__demo__/basic.md

@import ./__demo__/type.md

@import ./__demo__/icon.md

@import ./__demo__/position.md

@import ./__demo__/closeable.md

@import ./__demo__/update.md

### `Message` Global methods

The global methods provided by Message can be used in the following three ways:
1. Called by this.$message
2. In the Composition API, call getCurrentInstance().appContext.config.globalProperties.$message
3. Import Message and call it through Message itself


### MessageMethod

|Name|Description|Type|Default|
|---|---|---|:---:|
|info|Show info message|`(config: string \| MessageConfig) => MessageReturn`|`-`|
|success|Show success message|`(config: string \| MessageConfig) => MessageReturn`|`-`|
|warning|Show warning message|`(config: string \| MessageConfig) => MessageReturn`|`-`|
|error|Show error message|`(config: string \| MessageConfig) => MessageReturn`|`-`|
|clear|Clear all messages|`(position?: MessagePosition) => void`|`-`|



### MessageConfig

|Name|Description|Type|Default|
|---|---|---|:---:|
|content|Content|`RenderContent`|`-`|
|id|Unique id|`string`|`-`|
|icon|Message icon|`RenderFunction`|`-`|
|position|Location of the message|`'top'\|'bottom'`|`-`|
|showIcon|Whether to show icon|`boolean`|`false`|
|closable|Whether to show the close button|`boolean`|`false`|
|duration|The duration of the message display|`number`|`-`|



### MessageReturn

|Name|Description|Type|Default|
|---|---|---|:---:|
|close|Close current message|`() => void`|`-`|


