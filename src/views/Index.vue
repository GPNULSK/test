<template>
    <div class="main_div"   :style="totalBg">
        <div  class="login-container" :style="bg" style="height: 180px">

            <el-row :gutter="20" style="margin-top: 15px;">
                <el-col :span="22">
                    <div>
                        <el-input placeholder="请输入内容"  style="width: 500px;margin-top: 10px">
                            <el-button slot="append" icon="el-icon-search"></el-button>
                        </el-input>
                    </div>
                </el-col>
                <el-col :span="2">
                   <el-button style="margin-top: 10px">登录</el-button>
                </el-col>
            </el-row>
        </div>
            <div class="mid_ban">

            </div>
        <div>

        </div>

    </div>

</template>

<script>
    export default {
        name: "Index",
        data(){
            return{
                bg:{
                    backgroundImage:"url(" + require("../assets/topImg.png")+")",
                    backgroundRepeat: "no-repeat",
                },
                totalBg:{
                    backgroundImage:"url(" + require("../assets/totalBg.jpg")+")",
                    backgroundRepeat: "no-repeat",
                }
            }
        }
    }
</script>

<style scoped>

    .main_div{
        height: 1000px;
    }
    .mid_ban {
        width: 800px;
        height: 90px;
        background-color: rgb(255, 255, 255);
        border-radius: 15px;
        margin:  15px auto;
    }

</style>