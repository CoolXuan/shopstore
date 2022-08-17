<template>
  <div class="common-layout">
    <div class="myhead">
      <!-- 头部第一部分 网站信息 -->
      <header class="header">
        <div class="top">
          <div class="container">
            <div class="loginList">
              <p>小陈商城欢迎您</p>
              <p>
                <span>请</span>
                <a href="#">登录</a>
                <a href="#" class="register">免费注册</a>
              </p>
            </div>
            <div class="typeList">
              <a href="#">我的订单</a>
              <a href="#">我的购物车</a>
              <a href="#">我的商品</a>
              <a href="#">我的会员</a>
              <a href="#">企业采购</a>
              <a href="#">关注小陈商城</a>
              <a href="#">合作招商</a>
              <a href="#">商品后台</a>
            </div>
          </div>
        </div>
        <!-- 头部第二部分 搜索栏 -->
        <div class="bottom">
          <h1 class="logoArea">
            <a href="#" class="logo" title="小陈商城" target="_blank">
              <img src="./assets/logo.png" alt="" />
            </a>
          </h1>
          <div class="searcehArea">
            <form action="###" class="searchForm">
              <input
                type="text"
                name=""
                id="autocomplete"
                placeholder="请输入要查询商品"
                class="input-box"
              />
              <button class="btn search-btn">搜索</button>
            </form>
          </div>
        </div>
      </header>
    </div>
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
    <div class="myfoot">
      <ul>
        <li>
          <div class="footer-title">购物指南</div>
          <a href="#">购物流程</a>
          <a href="#">会员介绍</a>
          <a href="#">生活旅行</a>
          <a href="#">常见问题</a>
          <a href="#">购物中心</a>
        </li>
        <li>
          <div class="footer-title">配送方式</div>
          <a href="#">上门自费</a>
          <a href="#">24小时限时达</a>
          <a href="#">配送服务查询</a>
          <a href="#">官方配送收费标准</a>
          <a href="#">海外配送</a>
        </li>
        <li>
          <div class="footer-title">支付方式</div>
          <a href="#">货到付款</a>
          <a href="#">在线支付</a>
          <a href="#">分期付款</a>
          <a href="#">邮局汇款</a>
          <a href="#">公司转账</a>
        </li>
        <li>
          <div class="footer-title">售后服务</div>
          <a href="#">售后政策</a>
          <a href="#">价格保护</a>
          <a href="#">退款说明</a>
          <a href="#">返修/退换货</a>
          <a href="#">取消订单</a>
        </li>
        <li>
          <div class="footer-title">特色服务</div>
          <a href="#">夺宝岛</a>
          <a href="#">DIY装机</a>
          <a href="#">延保服务</a>
          <a href="#">商城E卡</a>
          <a href="#">人工客服</a>
        </li>
        <li>
          <div class="footer-title">帮助中心</div>
          <img src="codeimg" alt="codeimg" />
        </li>
      </ul>
    </div>
  </div>
</template>

<style lang="less">
* {
  padding: 0;
  margin: 0;
}
#app {
  font-family:Arial, Helvetica, sans-serif;
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

.myhead {
  border-radius: 5px;
  overflow: hidden;
  margin-bottom: 10px;
  font-weight: 600;
  background-color: rgb(246, 246, 246);
  margin-bottom: 10px;
  .header {
    width: 100%;
    height: auto;
    display: flex;
    flex-direction: column;
    .bottom {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      align-items: center;
      .logoArea {
        display: flex;
        flex-direction: row;
        justify-content: space-between;
        align-items: center;
        height: 87px;
        img {
          width: 50px;
          height: 50px;
        }
      }
      .searcehArea {
        .input-box {
          color: #fdb101;
          font-size: 5px;
          font-weight: 550;
          padding-left: 5px;
          border-radius: 5px;
          height: 22px;
          margin-right: 5px;
          border: solid gray 2px;
        }
        .input-box:focus {
          outline: none;
          border: 2px solid rgb(247, 191, 26);
        }
      }
    }

    .container {
      width: 100%;
      height: 30px;
      align-content: center;
      background-color: rgba(128, 128, 128, 0.475);
      display: flex;
      flex-direction: row;
      flex-wrap: nowrap;
      justify-content: space-between;
      align-items: center;
      a {
        width: auto;
        color: black;
        font-weight: 600;
        padding: 0 5px;
        // background-color: orange;
        border-right: 2px solid black;
        border-bottom: none;
        // border-right: solid rgb(255, 255, 255) 1px;
        list-style: none;
        text-decoration: none;
        position: relative;
        text-align: center;
        padding: 0 5px;
      }
      .loginList {
        width: 25%;
        display: flex;
        flex-direction: row;
        flex-wrap: nowrap;
        justify-content: space-between;
      }
    }
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
.myfoot {
  border-radius: 5px;
  overflow: hidden;
  margin-bottom: 10px;
  width: 100%;
  height: auto;
  background-color: rgb(161, 161, 161);
  ul {
    width: 100%;
    height: 100px;
    display: flex;
    flex-direction: row;
    justify-content: space-evenly;
    li {
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: flex-start;
      font-size: 12px;
      .footer-title {
        font-size: 14px;
        font-weight: 600;
      }
    }
  }
}
</style>
