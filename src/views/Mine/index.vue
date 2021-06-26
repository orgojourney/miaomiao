<template>
    <div id="main">
        <Header title="我的喵喵"></Header>
        <login />
        <Tabber></Tabber>
    </div>
</template>

<script>
import Header from '@/components/Header'
import Tabber from '@/components/Tabber'
import login from '@/components/login'


export default {
    name: 'Mine',
    components: {
        Header,
        Tabber,
        login
    }
}
</script>

<style scoped>

</style>