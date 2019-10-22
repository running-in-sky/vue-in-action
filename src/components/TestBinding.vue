<template>
    <div>
        <span v-if="showFlag" class="binding" >{{ msg }}</span>
        <a-button type="primary" @click="alertMsg()">{{showFlag ? '隐藏' : '显示'}}</a-button>
    </div>
</template>
<script>
    export default {
        name: 'TestBinding',
        data: function () {
            return {
                showFlag: true,
            }
        },
        methods: {
            alertMsg: function() {
                this.showFlag = !this.showFlag
            }
        },
        props: {
            msg: String
        }
    }
</script>

<style>
    .binding {
        padding: 10px;
    }
</style>