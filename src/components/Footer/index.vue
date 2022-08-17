<template>
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
        <img src="./images/logo.png" alt="codeimg" class="codeimg"/>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
    name:"MyFooter"
};
</script>

<style lang="less" scoped>
.myfoot {
    .codeimg{
        width: 70px;
        height: 70px;
    }
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
