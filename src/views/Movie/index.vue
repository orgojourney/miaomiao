<template>
    <div id="main">
        <Header title="喵喵电影"></Header>
        <Tabber></Tabber>
    </div>
</template>

<script>
import Header from '@/components/Header'
import Tabber from '@/components/Tabber'


export default {
    name: 'Movie',
    components: {
        Header,
        Tabber
    }
}
</script>

<style scoped>

</style>