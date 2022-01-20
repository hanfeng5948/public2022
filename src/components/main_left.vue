<template>
  <div class="mleft">
    <el-collapse
      v-model="activeNames"
      style="width: 240px; margin-left: 36px"
      @change="handleChange"
    >
      <el-collapse-item name="1" class="mycollapse">
        <template slot="title">
          <i class="menuicon span7" /><span>政策</span>
        </template>
        <div>
          与现实生活一致：与现实生活的流程、逻辑保持一致，遵循用户习惯的语言和概念；
        </div>
      </el-collapse-item>
      <el-collapse-item name="2" class="mycollapse">
        <template slot="title">
          <i class="menuicon span2" /><span>政府信息公开指南</span>
        </template>
        <div>
          控制反馈：通过界面样式和交互动效让用户可以清晰的感知自己的操作；
        </div>
      </el-collapse-item>
      <el-collapse-item name="3" class="mycollapse">
        <template slot="title">
          <i class="menuicon span3" /><span>政府信息公开制度</span>
        </template>
        <div>简化流程：设计简洁直观的操作流程；</div>
        <div>
          帮助用户识别：界面简单直白，让用户快速识别而非回忆，减少用户记忆负担。
        </div>
      </el-collapse-item>
      <el-collapse-item name="4" class="mycollapse">
        <template slot="title">
          <i class="menuicon span4" /><span>法定主动公开内容</span>
        </template>
        <div>
          用户决策：根据场景可给予用户操作建议或安全提示，但不能代替用户进行决策；
        </div>
      </el-collapse-item>
      <el-collapse-item name="5" class="mycollapse">
        <template slot="title">
          <i class="menuicon span5" /><span>政府信息公开年报</span>
        </template>
        <div>
          用户决策：根据场景可给予用户操作建议或安全提示，但不能代替用户进行决策；
        </div>
      </el-collapse-item>
      <el-collapse-item name="6" class="mycollapse">
        <template slot="title">
          <i class="menuicon span6" /><span>依申请公开</span>
        </template>
        <div>
          用户决策：根据场景可给予用户操作建议或安全提示，但不能代替用户进行决策；
        </div>
      </el-collapse-item>
      <el-collapse-item name="7" class="mycollapse">
        <template slot="title">
          <i class="menuicon span8" /><span>站点导航和专题</span>
        </template>
        <div>
          用户决策：根据场景可给予用户操作建议或安全提示，但不能代替用户进行决策；
        </div>
      </el-collapse-item>
    </el-collapse>
  </div>
</template>
<script>
export default {
  name: 'MainLeft',
  data() {
    return {
      activeNames: ['1']
    }
  },
  methods: {
    handleChange(val) {
      console.log(val)
    }
  }
}
</script>

<style scoped>
@import url("http://unpkg.com/element-ui@2.15.7/lib/theme-chalk/index.css");
 .mleft {
  background-color: rgb(242, 242, 242);
  margin-bottom: 15px;
}
/*.mleft >>> .el-collapse-item__header {
  background-color: #fff;
  color: #2d66a5;
  font-size: 23px;
  height: 70px;
  outline: none;
  line-height: 70px;
}
.mleft >>> .el-collapse-item__header.is-active {
  color: #fff;
  background-color: rgb(45, 102, 165);
}
.mleft >>> .el-collapse-item .menuicon {
    width: 100px;
    font-size: 35pt;
    line-height: 35pt;
    text-align: center;
}
.mleft >>> .el-collapse-item__header .span7::before {
  content: url('../assets/left_07.png');
}
.mycollapse .menuicon {
    width: 60px;
    text-align: center;
    font-size: 30pt;
}

.mleft >>> .el-collapse-item__header.is-active .span7::before {
  content: url('../assets/left1_07.png');
}
.mleft >>> .el-icon-arrow-right:before {
    font-size: 35px;
    margin-right: 5px;
    content: "\2B";
}
.mleft >>> .el-icon-arrow-right.is-active {
    font-size: 35px;
    line-height: 35px;
    margin-top: 10px auto;
    transform: rotate(180deg);
}
.mleft >>> .el-icon-arrow-right.is-active::before {
    content: "\2013";
} */

.mleft >>> .el-collapse-item__header {
    font-size: 23px;
    line-height: 23px;
    height: 70px;
    background-color: rgb(255, 255, 255);
    margin-bottom: 15px;
    border: 1px solid #ddd;
    color: #2d66a5;

}
.mleft >>> .el-collapse-item__header.is-active {
    background-color: rgb(45, 102, 165);
    color: #fff;
}
.mycollapse .menuicon {
    width: 80px;
    text-align: center;
    font-size: 30pt;
}
.mycollapse i.span2::before {
    content: url("../assets/left_02.png");
}
.mycollapse .is-active i.span2::before {
    content: url("../assets/left1_02.png");
}
.mycollapse i.span3::before {
    content: url("../assets/left_03.png");
}
.mycollapse .is-active i.span3::before {
    content: url("../assets/left1_03.png");
}
.mycollapse i.span4::before {
    content: url("../assets/left_04.png");
}
.mycollapse .is-active i.span4::before {
    content: url("../assets/left1_04.png");
}
.mycollapse i.span5::before {
    content: url("../assets/left_05.png");
}
.mycollapse .is-active i.span5::before {
    content: url("../assets/left1_05.png");
}
.mycollapse i.span6::before {
    content: url("../assets/left_06.png");
}
.mycollapse .is-active i.span6::before {
    content: url("../assets/left1_06.png");
}
.mycollapse i.span8::before {
    content: url("../assets/left_08.png");
}
.mycollapse .is-active i.span8::before {
    content: url("../assets/left1_08.png");
}

.mycollapse i.span7::before {
    content: url("../assets/left_07.png");
}
.mycollapse .is-active i.span7::before {
    content: url("../assets/left1_07.png");
}

.mycollapse span {
    width: 100px;
    text-align: justify;
    text-align-last:justify;
}

.container_body {
    background-color:rgb(242,242,242);
}
.mleft >>> .el-collapse-item .el-icon-arrow-right:before {
    font-size: 35px;
    content: "\2B";
    line-height: 35px;
}
.mleft >>> .el-collapse-item .el-icon-arrow-right.is-active {
    font-size: 35px;
    padding-bottom: 10px;
    padding-left: 4px;
    transform: rotate(180deg);
}
.mleft >>> .el-collapse-item .el-icon-arrow-right.is-active::before {
    content: "\2013";
}
</style>
