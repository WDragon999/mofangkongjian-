<template>
    <div id="homePage">
        <div class="navbar-header">
            <a class="navbar-brand" href="#">
                <img alt="Brand" class="navbar-img" src="../img/logo.png">
            </a>
            <div class="audition">
                <div class="audition-button" @click='audition'>
                    <!-- <a href="">免费领取价值188元试听课</a> -->
                    免费领取价值188元试听课
                </div>
            </div>
        </div>
        <div class="content-box">
            <div class="img_box" style="margin-top:120px">
                <img alt="Brand" class="" src="../img/图片1.png">
            </div>
            <div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片2.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片3.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片4.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片5.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片6.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片7.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片8.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片9.png">
                </div>
                <div class="img_box_inside">
                    <img alt="Brand" class="img" src="../img/图片10.png">
                </div>
            </div>
        </div>
        <div class="audition-box" v-if='isshowaudition'>
            <div class="audition-box-content">
                <div class="close" @click='audition'>X</div>
                <img src="../img/添加工作人员.jpg" class="add-wechat" alt="">
                <h1>扫描二维码添加客服微信</h1>
            </div>
        </div>
        <div class="bottom_box">
            备案信息
            成都达达虎科技有限公司
            版权所有
            公司地址
            联系方式
        </div>
    </div>
</template>

<script>

export default {
  name: 'homePage',
  data () {
    return {
    //   msg: 'Welcome to Your Vue.js App',
      isshowaudition: false
    }
  },
  methods: {
    audition () {
      console.log(11111)
      this.isshowaudition ? this.isshowaudition = false : this.isshowaudition = true
    }
  }
}

</script>

<style scoped>
.navbar-header{
    position: fixed;
    width: 100%;
    height: 120px;
    background: gray;
    top:0;
    box-shadow: 0 10px 5px;
    vertical-align: middle;
}
.audition{
    /* display: inline-block; */
    float: right;
    width: 300px;
    height: 120px;
    margin-right: 300px;
    padding-top: 40px;
}
.audition-button{
    line-height: 50px;
    border-radius: 30px;
    background: red;
    color: white;
    cursor: pointer;
}
.close{
    float: right;
    margin-right: 10px;
    margin-top: 10px;
    cursor: pointer;
}
.navbar-brand{
    margin:0 auto;
}
.navbar-brand img{
    height: 90px;
    margin-top: 20px;
}
.img_box{
    width: 100%;
}
.img_box img{
    width: 100%;
}
.img_box_inside{
    width: 60%;
    margin: auto;
    box-shadow: 10px seashell;
}
.audition-box{
    position: fixed;
    top: 0;
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.5);
}
.audition-box-content{
    width: 500px;
    height: 500px;
    background: white;
    margin: auto;
    margin-top: 200px;
}
.add-wechat{
    width: 450px;
    height: 400px;
    margin-top: 20px;
    margin-left: 20px;
    /* margin:auto */
}
.bottom_box{
    height: 300px;
    background: black;
    color: blanchedalmond;
}
</style>
