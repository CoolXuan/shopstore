<template>
  <div class="common-layout">
    <MyHeader />
    <div class="mymain">
      <div class="nav-main">
        <ul>
          <li class="all-shop"><a href="#">全部商品分类</a></li>
          <li><a href="#">服装城</a></li>
          <li><a href="#">美妆馆</a></li>
          <li><a href="#">小陈超市</a></li>
          <li><a href="#">全球购</a></li>
          <li><a href="#">闪购</a></li>
          <li><a href="#">团购</a></li>
          <li><a href="#">有趣</a></li>
          <li><a href="#">秒杀</a></li>
        </ul>
      </div>
      <div class="main-content">
        <div class="main-left">
          <div class="main-nav">
            <a href="#">衣服裤子</a>
            <a href="#">家电装修</a>
            <a href="#">日用产品</a>
            <a href="#">个护化妆</a>
            <a href="#">手机数码</a>
            <a href="#">电脑办公</a>
            <a href="#">运动体育</a>
            <a href="#">箱包鞋盒</a>
            <a href="#">母婴玩具</a>
            <a href="#">彩票旅行</a>
          </div>
        </div>
        <div class="main-center">
          <el-carousel trigger="click" height="500px">
            <el-carousel-item v-for="item in 4" :key="item">
              <h3 class="small justify-center" text="2xl">{{ item }}</h3>
            </el-carousel-item>
          </el-carousel>
        </div>
        <div class="main-right">3</div>
      </div>
    </div>
    <MyFooter />
  </div>
</template>
<script>
import MyFooter from "./components/Footer";
import MyHeader from "./components/Header";
export default {
  name: "app",
  components: {
    MyFooter,
    MyHeader,
  },
};
</script>
<style lang="less">
* {
  padding: 0;
  margin: 0;
}
#app {
  font-family: Arial, Helvetica, sans-serif;
  font-size: 12px;
  width: 1000px;
  height: auto;
  margin: 0 auto;
  .btn {
    border-radius: 5px;
    margin: 5px;
    width: 50px;
    height: 25px;
    color: rgb(64, 64, 64);
    font-weight: 600;
    background-color: rgb(44, 255, 79);
  }
  a {
    // background-color: orange;
    // border-right: solid rgb(255, 255, 255) 1px;
    list-style: none;
    text-decoration: none;
    position: relative;
    text-align: center;
    color: black;
  }
  li {
    list-style: none;
  }
}

.mymain {
  border-radius: 5px;
  overflow: hidden;
  margin-bottom: 10px;
  width: 100%;
  height: auto;
  // background-color: yellow;
  display: flex;
  flex-direction: column;
  .main-content {
    height: 500px;
    display: flex;
    flex-direction: row;
    .main-left {
      width: 18%;
      height: 500px;
      // background-color: red;
      .main-nav {
        display: flex;
        flex-direction: column;
        margin-top: 2px;
        a {
          display: flex;
          justify-content: center;
          align-items: center;
          width: 100%;
          height: 40px;
          background-color: rgb(238, 238, 238);
        }
        a:hover {
          font-size: medium;
          font-weight: 600;
        }
      }
    }
    .main-center {
      flex: 3;
      height: 100%;
      background-color: rgb(162, 255, 1);
      .demonstration {
        color: var(--el-text-color-secondary);
      }
      // 轮播图
      .el-carousel__item h3 {
        color: #475669;
        opacity: 0.75;
        line-height: 150px;
        margin: 0;
        text-align: center;
      }

      .el-carousel__item:nth-child(2n) {
        background-color: #99a9bf;
      }

      .el-carousel__item:nth-child(2n + 1) {
        background-color: #d3dce6;
      }
    }
    .main-right {
      flex: 1;
      height: 100%;
      background-color: rgb(68, 0, 255);
    }
  }
  .nav-main {
    height: 40px;
    line-height: 40px;
    border-radius: 5px;
    overflow: hidden;
    ul {
      list-style: none;
      display: flex;
      flex-direction: row;
      justify-content: left;
      border-bottom: orange solid 2px;
      background-color: rgb(176, 211, 0);
      li {
        width: auto;
        padding: 0 15px;
        font-size: 14px;
        // background-color: #fff;
      }
      li:hover {
        font-size: 20;
        font-weight: 600;
        // border-bottom: solid blue 2px;
        background-color: rgb(255, 202, 56);
      }
      .all-shop {
        width: 150px;
        text-align: center;
      }
    }
  }
}
</style>
