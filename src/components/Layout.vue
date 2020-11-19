<template>

    <el-container>
        <el-header>
            这里是标题
        </el-header>
        <el-main>
            <el-container>

                <el-aside>
                    <el-menu>
                        <el-submenu>
                            <el-menu-item>
                                <router-link to="/">Home</router-link>
                            </el-menu-item>
                            <el-menu-item-group>
                                <el-menu-item>
                                    <router-link to="/about">About</router-link>
                                </el-menu-item>
                                <el-menu-item>
                                    <router-link to="/other">Other</router-link>
                                </el-menu-item>
                            </el-menu-item-group>
                        </el-submenu>
                    </el-menu>
                </el-aside>
                <el-main>
                    <router-view/>
                </el-main>
            </el-container>

        </el-main>


    </el-container>

</template>


<script>


    export default {
        name: 'layout',
        components: {}
    }
</script>