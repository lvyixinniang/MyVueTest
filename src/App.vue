<template>
    <h3>模版语法</h3>
    <p>{{ msg }}</p>
    <h2>{{ number + 1 }}</h2>
    <p>{{ !flag }}</p>
    <h3>{{ flag ? "YES":"NO" }}</h3>
    <div>{{ message.split("").reverse().join("") }}</div>
    <p v-html="trunHref"></p>
</template>

<script>
export default{
    data(){
        return{
            msg:"神奇的魔法",
            number:10,
            flag:true,
            message:"大家好",
            trunHref:"<a href='https://www.bing.com'>必应<a/>"
        }
    }
}
</script>
