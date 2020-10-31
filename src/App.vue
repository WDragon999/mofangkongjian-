<template>
  <div id="app">
    22222
    <home-page></home-page>
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
*{
    margin: 0;
    padding: 0;
}
html {
    overflow-y: scroll;
}

:root {
    overflow-y: auto;
    overflow-x: hidden;
}

:root body {
    position: absolute;
}

body {
    width: 100vw;
    min-width: 1500px;
    overflow: hidden;
}
a{
    text-decoration: none;
}
.navbar{
    min-height:80px;
    margin-bottom: 0px;
}
@media (min-width: 768px){
    .navbar-collapse.collapse {
        height: 80px!important;
    }
}
.container-fluid,.navbar-brand{
    height:80px;
    padding: 0px;
    line-height: 80px;
}
@media (min-width: 768px){
     .container-fluid>.navbar-header{
        margin-left: 160px;
    }
}
.navbar-brand img{
    width:150px;
    height:80px;
}
.nav_link{
    width:820px;
    height:80px;
    float: right;
    margin-right: 160px;
}
.nav_ul{
    height:80px;
    margin-bottom: 0px;
}
.nav_ul,.nav_ul li{
    display: inline-block;
}
.nav_ul li{
    width: 120px;
    height:80px;
    list-style-type: none;
}
.nav_ul li a,.li_span{
    margin-top: 15px;
    width: 120px;
    height:50px;
}
.li_span{
    color: #5a5a5a;
    text-align: center;
    line-height: 50px;
    font-size: 14px;
    display: block;
    overflow: hidden;
}
.nav_ul a:hover{
    color:#FFB44B;
}
.li_span:hover{
    background-color: #FFB44B;
    border-radius: 25px;
    font-weight: bold;
    color: #fff;
    font-size: 16px;
}
.tel{
    width: 300px;
    height:400px;
    background-color: rgba(255,255,255,0);
    color: #fff;
    position: absolute;
    font-size: 40px;
    top:150px;
    right:100px;
}
.tel p{
    margin-top: 10px;
}
.p1{
    font-size: 60px;
}
.tel_input{
    width: 300px;
    height: 55px;
    background-color: #fff;
    border: 1px solid #E8631C;
    position: relative;
    z-index: 1;
}
.tel_input span{
    width:45px;
    height:55px;
    position: relative;
    color: #cccccc;
    text-align: center;
    line-height: 55px;
    z-index: 2;
}
.tel_input input{
    width:255px;
    height:55px;
    position: absolute;
    border: 1px solid #E8631C;
    border-left: 0;
    color: #000;
    top:-1px;
    left:45px;
    font-size: 25px;
}
.addInfo{
    font-size: 12px;
    /*border:1px solid red;*/
    position: absolute;
    left:-55px;
    top:20px;
}
#class_btn{
    width: 300px;
    height: 55px;
    line-height:41px;
    border: 1px solid #E8631C;
    background-color: #E8631C;
    color: #fff;
    font-size: 25px;
    position: relative;
    left:-120px;
    top:0;
}
#class_btn:hover{
    border: 1px solid #FFE84A;
    background-color: #FFE84A;
}
.our_server{
    width: 100%;
    height:600px;
    background-color: #FFB44B;
}
.our_server h1,.our_server p{
    font-family: 微软雅黑;
    text-align: center;
    color: #fff;
}
.our_server h1{
    font-size: 35px;
    margin:0px;
    padding-top: 60px;
}
.our_server p{
    font-size: 25px;
}
.service{
    width: 1200px;
    height:600px;
    margin:50px auto;
    margin-bottom: 0px;
    display: flex;
    flex-direction: row;
    flex-wrap: wrap;
    justify-content: space-around;
}
.service_item{
    width: 400px;
    height:300px;
    /*border: 1px solid red;*/
    flex-shrink:0;
}
.item_1{
    background-color: #8DDFFF;
}
.item_img{
    width: 68px;
    height:70px;
    margin:40px 166px 15px 166px;
}
.item_img img{
    width: 68px;
    height:70px;
}
.item_1 p{
    font-size: 20px;
}
.btn{
    width:160px;
    height:50px;
    border-radius: 25px;
    line-height: 50px;
    text-align: center;
    font-size: 14px;
    margin:30px 120px 120px;
}
.btn_color1{
    background-color: #fff;
}
.btn div{
    width:154px;
    height:44px;
    border-radius: 22px;
    line-height: 44px;
    text-align: center;
    font-size: 14px;
    position: relative;
    left:-10px;
    top:-4px;
}
.div_color1{
    background-color: #8DDFFF;
}
.btn a{
    color: #fff;
}
.item_2 img{
    width: 400px;
    height:300px;
}
.item_3{
    background-color: #fff;
}
.btn_color2{
    background-color: #ccc;
}
.div_color2{
    background-color: #fff;
}
.div_color2 a{
    color: black;
}
.item_3 p{
    color: #000;
    font-size: 20px;
}
.item_4{
    background-color: #37C093;
}
.item_4 p{
    font-size: 20px;
}
.btn_color3{
    background-color: #fff;
}
.div_color3{
    background-color: #37C093;
}
.about_us{
    width: 100%;
    height: 400px;
    margin-top: 300px;
}
.about_us img{
    width: 100%;
    height: 400px;
}
footer{
    width: 100%;
    height:50px;
    margin-top: 300px;
    color: #000;
    line-height: 50px;
    text-align: center;
    background-color: #F2F2F2;
}
footer p{
    margin-bottom: 0;
}

</style>
