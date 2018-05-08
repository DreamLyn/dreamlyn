<template>
    <div id="app">
        <el-menu :default-active="activeIndex1" class="el-menu-demo" mode="horizontal" @select="handleSelect" background-color="#545c64" text-color="#fff" active-text-color="#ffd04b">
            <el-menu-item v-for="(option,index) in menu" :index="index">{{option.label}}</el-menu-item>

        </el-menu>
        <router-view/>
    </div>
</template>

<script>
export default {
    name: "App",
    data() {
        return {
            menu: [
                {
                    label: "嵌入式工具集"
                },
                {
                    label: "程序员工具集"
                },
                {
                    label: "会计工具集"
                },
                {
                    label: "金融工具集"
                },
                {
                    label: "汽车工具集"
                }
            ]
        };
    }
};
</script>


<style>
#app {
    font-family: "Avenir", Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 0px;
}
</style>
