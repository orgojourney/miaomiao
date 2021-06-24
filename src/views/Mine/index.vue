<template>
    <div id="main">
        <Header title="我的喵喵"></Header>
        <Tabber></Tabber>
    </div>
</template>

<script>
import Header from '@/components/Header'
import Tabber from '@/components/Tabber'


export default {
    name: 'Mine',
    components: {
        Header,
        Tabber
    }
}
</script>

<style scoped>

</style>