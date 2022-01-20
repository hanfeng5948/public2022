<template>
  <div class="container" style="width: 1100px; margin: 0 auto; ">
    <!-- <el-container :direction="vertical">

                <div>
                    <a :href="base_url">
                        <img style="height:70px; width:70px;" src="../assets/gknew_logo.png" @click="clk"></img>
                    </a>
                </div>
                <div>
                    <a :href="l_url">
                        枞阳县人民政府(县政府办公室)
                    </a>
                </div>
            </el-container> -->
    <el-header height="365">
      <el-row :gutter="0" type="flex" justify="left" style="display:flex;flex-wrap: wrap;">
        <el-col :span="3" :offset="0">
          <div class="gknew_logo">
            <a :href="base_url">
              <img style="height:70px; width:70px;" src="../assets/gknew_logo.png"></img>
            </a>
          </div>
        </el-col>
        <el-col :span="21" :offset="0">
          <div class="unit_name">
            <a :href="l_url">
              枞阳县人民政府(县政府办公室)
            </a>
          </div>
        </el-col>
      </el-row>
      <el-row :gutter="0">
        <el-col :span="24" :offset="0">
          <ul class="gknew_ban" />
        </el-col>
      </el-row>
    </el-header>

  </div>

</template>

<script>
export default {
  name: 'ZHeader',
  props: {
    unitid: {
      type: Number,
      default: 5
    }
  },
  data: function() {
    return {
      base_url: 'http://zfxxgk.zongyang.gov.cn',
      ex_url: '/public/index_66.aspx?unitid=',
      l_url: this.base_url + this.ex_url + this.unitid
    }
  },
  methods: {
    clk() {
      console.log(this.base_url)
    }
  }
}
</script>
<style scoped>
.container {
    margin-right: auto;
    margin-left: auto;
    padding-top: 10px;
    padding-left: 0;
    padding-right: 0;
    width: 1100px;
    height: 365px;
}
.gk_banner {
    padding: 20px 0 105px;
    margin: 0 50px;
}
.gk_container {
    max-width: 1028px;
    margin: 0 auto;
    padding: 80px 36px 25px;
}
.gkwz_container {
    max-width: 1100px;
    margin: 0 auto;
    padding: 0 0 10px;
}
.gknew_logo {
    text-align: center;
    /* padding-left: 85px; */
    font-size: 35px;
    /* background: url("../assets/gknew_logo.png") left center no-repeat; */
    font-weight: bold;
    color: #fff;
    line-height: 50px;
    height: 76px;
}
.unit_name {
    text-align: left;
    font-size: 35pt;
    font-family: "微软雅黑", "Microsoft YaHei", Arial, sans-serif;
    font-weight: bolder;
    padding: auto 0;
}
.unit_name a {
    color: #fff;
    text-decoration: none;
}
.gknew_ban {
    background: url("../assets/pic-banner.png") center 0 no-repeat;
    height: 104px;
    margin-top: 83px;
}
.gk_container {
    padding: 80px 36px 25px;
    max-width: 1028px;
    margin: 0 auto;
    background: #fff;
}
@media (max-width: 1099px) and (min-width: 992px) {
    .gk_banner {
        padding-bottom: 80px;
        margin: 0;
    }
}
@media only screen and (max-width: 991px) {
    .gk_container {
        padding: 20px 10px 10px;
    }
}
@media (max-width: 991px) and (min-width: 768px) {
    .gk_banner {
        padding-bottom: 50px;
        margin: 0;
    }
    .gknew_logo {
        font-size: 22px;
        line-height: 28px;
        background-size: auto 40px;
        padding: 6px 0 6px 50px;
        height: auto;
    }
}
@media (max-width: 767px) {
    .gknew_ban {
        text-align: center;
        margin-top: 30px;
        background-size: auto 100%;
        height: 45px;
    }
    .gk_banner {
        padding: 20px 10px 40px;
        margin: 0;
    }
    .gknew_logo {
        font-size: 22px;
        line-height: 28px;
        background-size: auto 40px;
        padding: 6px 0 6px 50px;
        height: auto;
    }
}
</style>
