<template>
  <el-container>
<!--    <el-aside>-->
<!--      <el-row class="tac">-->
<!--        <el-col :span="12">-->
<!--          <el-menu-->
<!--            default-active="2"-->
<!--            class="el-menu-vertical-demo"-->
<!--            @open="handleOpen"-->
<!--            @close="handleClose"-->
<!--            background-color="#545c64"-->
<!--            text-color="#fff"-->
<!--            active-text-color="#ffd04b">-->
<!--            <el-submenu index="1">-->
<!--              <template slot="title">-->
<!--                <i class="el-icon-location"></i>-->
<!--                <span>导航一</span>-->
<!--              </template>-->
<!--              <el-menu-item-group>-->
<!--                <template slot="title">分组一</template>-->
<!--                <el-menu-item index="1-1">选项1</el-menu-item>-->
<!--                <el-menu-item index="1-2">选项2</el-menu-item>-->
<!--              </el-menu-item-group>-->
<!--              <el-menu-item-group title="分组2">-->
<!--                <el-menu-item index="1-3">选项3</el-menu-item>-->
<!--              </el-menu-item-group>-->
<!--              <el-submenu index="1-4">-->
<!--                <template slot="title">选项4</template>-->
<!--                <el-menu-item index="1-4-1">选项1</el-menu-item>-->
<!--              </el-submenu>-->
<!--            </el-submenu>-->
<!--            <el-menu-item index="2">-->
<!--              <i class="el-icon-menu"></i>-->
<!--              <span slot="title">导航二</span>-->
<!--            </el-menu-item>-->
<!--            <el-menu-item index="3" disabled>-->
<!--              <i class="el-icon-document"></i>-->
<!--              <span slot="title">导航三</span>-->
<!--            </el-menu-item>-->
<!--            <el-menu-item index="4">-->
<!--              <i class="el-icon-setting"></i>-->
<!--              <span slot="title">导航四</span>-->
<!--            </el-menu-item>-->
<!--          </el-menu>-->
<!--        </el-col>-->
<!--      </el-row>-->
<!--    </el-aside>-->
    <el-main>
      <div align="center">

          <Content :style="{margin: '20px 160px 0'}">
            <VideoPlay/>
          </Content>

      </div>
    </el-main>
  </el-container>
</template>

<style scoped>
.layout{
  border: 0px solid #dcdee2;
  position: relative;
  border-radius: 4px;
  overflow: hidden;
}
.layout-header-bar{
  box-shadow: 0 1px 1px rgba(0,0,0,.1);
}
.div-bar{
  margin-left: 200px;
}
</style>

<script>

import VideoPlay from "./VideoPlay";
import infomation from "./infomation";
export default {
  components: {
    VideoPlay,
    infomation
  },
  methods:{
    handleClose(){
      console.log("close方法")
    },
    handleOpen(){
      console.log("open方法")
    },
  },
  data() {
      return {

      }
    }
  };
</script>
