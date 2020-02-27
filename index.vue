<template>
    <button :class="classes( [ this.type, this.size, {
                loading: this.loading,
                disabled: this.disabled,
                hairline: this.hairline,
                block: this.block,
                plain: this.plain,
                round: this.round,
                square: this.square
            } ] )" @click="handleClick">
        <span class="hanzo-button__text"><slot>{{text}}</slot></span>
    </button>
</template>

<script>
import { classesMixin } from '../mixins/classname';
let classMixin = classesMixin('button');
export default {
    mixins: [classMixin],
    name: "h-button",
    props: {
        text: String,
        block: Boolean,
        plain: Boolean,
        round: Boolean,
        square: Boolean,
        loading: Boolean,
        hairline: Boolean,
        disabled: Boolean,
        loadingText: String,
        loadingType: String,
        type: {
            type: String,
            default: 'default'
        },
        size: {
            type: String,
            default: 'normal'
        },
        loadingSize: {
            type: String,
            default: '20px'
        }
    },
    methods: {
        handleClick( e ) {
            if ( !this.loading && !this.disabled ) {
                this.$emit( 'click', e );
            }
        }
    }
}
</script>

<style lang="less">
@import './index.less';
</style>