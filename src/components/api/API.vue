两级菜单，cmd，action，来选择协议。


选择完成两级菜单后，下方展示参数Form，

用户填写Form，点击执行按钮。


下方返回结果。


数据里面，定义了参数和结果的描述。


根据描述，展示不同的UI。


<template>
    <Selector></Selector>
    <button></button>
    <RequestForm></RequestForm>
    <ResponseForm></ResponseForm>
</template>


<script>
    export default {
        data() {
            return {}
        }
    }
</script>
