<template>
  <div class="header">
    <div class="h-1">
      <a href="/"><img :src="logo"></a>
    </div>
    <div class="h-2">
      <h1>虹扬专业精神  焕发创意力量</h1>
    </div>
    <div class="h-3">
      <ul v-for="item in menu">
        <li><a :href="item.link" >{{item.title}}</a></li>
      </ul>
    </div>
    <div class="h-4">
      <a href="/"><div class="h-4-b-1"><img src="../assets/imges/erweima.jpg"></div></a>
      <a href="/"><div class="h-4-b-2"><img src="../assets/imges/button1.png"></div></a>
    </div>
  </div>
</template>

<script>
    export default {
        name: "Header",
        data(){
            return {
                logo:"../static/logo.png",
                title:"",
                menu:[
                    {
                        title:"首页",
                        link:"/index",
                    },
                    {
                        title:"虹焕优势",
                        link:"/youshi",
                    },
                    {
                        title:"虹焕案例",
                        link:"/anli",
                    },
                    {
                        title:"关于虹焕",
                        link:"/about",
                    },
                    {
                        title:"虹焕动态",
                        link:"/dongtai",
                    },
                    {
                        title:"联系虹焕",
                        link:"/lianxi",
                    }
                ],
            }
        }
    }
</script>

<style scoped>

</style>
