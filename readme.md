#### API

|   参数   |                        说明                        |   类型    |  默认值   | 版本  |
| :------: | :------------------------------------------------: | :-------: | :-------: | :---: |
|   type   | 类型，可选值为 `primary` `info` `warning` `danger` `gray` | `String`  | `default` | 0.1.0 |
|   size   |       尺寸，可选值为 `large` `small` `mini`        | `String`  | `normal`  | 0.1.0 |
|   text   |                        文字                        | `String`  |     -     | 0.1.0 |
|  block   |                   是否为块级元素                   | `Boolean` |  `false`  | 0.1.0 |
|  plain   |                   是否为朴素按钮                   | `Boolean` |  `false`  | 0.1.0 |
|  square  |                   是否为方形按钮                   | `Boolean` |  `false`  | 0.1.0 |
|  round   |                   是否为圆形按钮                   | `Boolean` |  `false`  | 0.1.0 |
| disabled |                    是否禁用按钮                    | `Boolean` |  `false`  | 0.1.0 |
| hairline |                是否使用 0.5px 边框                 | `Boolean` |  `false`  | 0.1.0 |

#### Event

| 事件名 | 说明                                     | 参数         | 版本  |
| ------ | ---------------------------------------- | ------------ | ----- |
| click  | 点击按钮，且按钮状态不为加载或禁用时触发 | event: Event | 0.1.0 |

