<template>
    <div class="navbar">
        <div class="navbar__item" v-for="item in list" :key="item.id" @click="$emit('changeCategory',item)"
        >{{item.name}}</div>
    </div>
</template>
<script>
import api from '@/js/api'
export default {
    data() {
        return {
            list:[]
        }
    },
    created(){
        this.getItems();
    },
    methods:{
        getItems(){
            this.$axios.get(api.CategoryApi).then(res=> {
                this.list = res.data;
            });
        }
    }
}
</script>
<style scoped>
.navbar{
    min-width: 300px;
    border: 1px solid #ccc;
    border-radius: 8px;
    background: #fff;
    height: 100%;
    display: flex;
    flex-wrap: wrap;
}
.navbar__item{
    display: block;
    width: 20%;
    height: 50px;
    line-height: 50px;
    text-align: left;
    padding: 0 24px;
    transition: all linear 1s;
    cursor: pointer;
}
.navbar__item:hover{
    background: #d90429;
}
</style>