### 按钮

<template>
    <div>
        <h4>按钮类型</h4>
        <h-button type="default">默认按钮</h-button>
        <h-button type="primary">主要按钮</h-button>
        <h-button type="info">信息按钮</h-button>
        <h-button type="warning">警告按钮</h-button>
        <h-button type="danger">危险按钮</h-button>
        <h-button type="gray">危险按钮</h-button>
    </div>
    <div>
        <h4>朴素按钮</h4>
        <h-button plain type="primary">朴素按钮</h-button>
        <h-button plain type="danger">朴素按钮</h-button>
    </div>
    <div>
        <h4>按钮形状</h4>
        <h-button square type="primary">方形按钮</h-button>
        <h-button round type="danger">圆形按钮</h-button>
    </div>
    <div>
        <h4>按钮尺寸</h4>
        <h-button size="large">大号按钮</h-button>
        <h-button size="normal">普通按钮</h-button>
        <h-button size="small">小型按钮</h-button>
        <h-button size="mini">迷你按钮</h-button>
    </div>
    <div>
        <h4>按钮边框</h4>
        <h-button plain hairline type="primary">细边框按钮</h-button>
        <h-button plain hairline type="danger">细边框按钮</h-button>
    </div>
    <div>
        <h4>禁用状态</h4>
        <h-button type="default" disabled>默认按钮</h-button>
        <h-button type="primary" disabled>主要按钮</h-button>
        <h-button type="info" disabled>信息按钮</h-button>
    </div>
</template>

<script>
import hButton from './index'
export default {
    name: "button-demo",
    data() {
        return {
            type: 'primary'
        }
    },
    components: {
        hButton
    },
    methods: {
        aa() {
            this.type = 'warning'
        }
    }
}
</script>

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

