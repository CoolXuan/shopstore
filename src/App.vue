<template>
  <div class="common-layout">
    <el-container>
      <el-header class="myhead">
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
                <input type="text" name="" id="autocomplete" class="" />
                <button class="btn search-btn">搜索</button>
              </form>
            </div>
          </div>
        </header>
      </el-header>
      <el-main class="mymain">Main</el-main>
      <el-footer class="myfoot">Footer</el-footer>
    </el-container>
  </div>
</template>

<style lang="less">
* {
  padding: 0;
  margin: 0;
}
#app {
  font-family: "Courier New", Courier, monospace;
  font-size: 12px;
  width: 1000px;
  height: auto;
  margin: 0 auto;
}

.myhead {
  font-weight: 600;
  background-color: rgb(246, 246, 246);
  margin-bottom: 10px;
  .header {
    width: 100%;
    height: 100px;
    display: flex;
    flex-direction: column;
    .bottom {
      display: flex;
      flex-direction: row;
      justify-content: space-between;
      line-height: 50px;
      .logoArea {
        img {
          width: 50px;
          height: 50px;
        }
      }
    }

    .container {
      width: 100%;
      height: 20px;
      line-height: 23px;
      align-content: center;
      background-color: rgba(128, 128, 128, 0.475);
      display: flex;
      flex-direction: row;
      flex-wrap: nowrap;
      justify-content: space-between;
      a {
        width: auto;
        color: black;
        font-weight: 600;
        line-height: 20px;
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
  width: 100%;
  height: auto;
  background-color: yellow;
}
.myfoot {
  background-color: blue;
}
</style>
