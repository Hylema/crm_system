<template>
    <v-container fluid style="height: 100%; padding: 0px">
        <v-layout align-center justify-center column fill-height>
            <div>
                <strong :style="window.width > 1000 ? {'font-size': '150px'} : {'font-size': '50px'}">{{ name }}</strong>
            </div>
            <div style="text-align: center">
                <strong :style="window.width > 1000 ? {'font-size': '100px'} : {'font-size': '30px'}">Такой страницы не существует</strong>
            </div>
        </v-layout>
    </v-container>
</template>

<script>
    import windowSize from '../../mixins/windowSize'
    export default {
        name: "NotFound",
        mixins: [windowSize],
        data()  {
            return {
                name: '404',
            }
        }
    }
</script>

<style scoped>

</style>
