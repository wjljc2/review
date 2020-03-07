<template>
    <div>
        Mine component.
        <!-- {{$route.params.id}}
        {{$route.params.name}} -->

        {{$route.query.id}}
        {{$route.query.name}}
        <router-link to="/mine/test1">子路由1 |</router-link>
        <router-link to="/mine/test2">子路由2</router-link>
        <router-view></router-view>
    </div>
</template>

<script>
    export default {
        data(){
            return{
                msg:'haha'
            }
        },
        methods:{

        },
        created(){
            console.log(this.msg);
            console.log(this.$route.params.id);
        }
    }
</script>

<style lang="scss" scoped>

</style>