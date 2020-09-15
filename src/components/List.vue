<template>
<div>
<div v-bind:key="list.id" v-for="list in lists">
<ListItem v-bind:list="list" />
</div>
</div>
</template>

<script>
import ListItem from './ListItem.vue'

export default {
    name:"List",

components:{
        ListItem
    },

    props:["lists"]
}
</script>

<style lang="less" scoped>

</style>