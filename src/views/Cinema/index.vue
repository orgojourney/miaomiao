<template>
    <div id="main" >
        <Header title="喵喵影院"></Header>
        <Tabber></Tabber>
    </div>
</template>

<script>
import Header from '@/components/Header'
import Tabber from '@/components/Tabber'


export default {
    name: 'Cinema',
    components: {
        Header,
        Tabber
    }
}
</script>

<style scoped>

</style>