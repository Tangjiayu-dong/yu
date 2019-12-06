<template>
  <div class="home">
    <div class="header">
      <h3>多加网</h3>
      <input type="text" placeholder="请输入关键字"/>
    </div>
    <div class="main">
      <van-swipe :autoplay="3000" indicator-color="white">
        <van-swipe-item>1</van-swipe-item>
        <van-swipe-item>2</van-swipe-item>
        <van-swipe-item>3</van-swipe-item>
        <van-swipe-item>4</van-swipe-item>
      </van-swipe>
      <van-card
        num="2"
        price="2.00"
        desc="描述信息"
        title="商品标题"
        thumb="https://img.yzcdn.cn/vant/t-thirt.jpg"
      />
       <van-card
        num="2"
        price="2.00"
        desc="描述信息"
        title="商品标题"
        thumb="https://img.yzcdn.cn/vant/t-thirt.jpg"
      />
       <van-card
        num="2"
        price="2.00"
        desc="描述信息"
        title="商品标题"
        thumb="https://img.yzcdn.cn/vant/t-thirt.jpg"
      />
    </div>
    <div class="footer">
      <router-link to="/home" tag="span">首页</router-link>
      <router-link to="/my" tag="span">我的</router-link>
    </div>
    <router-view />
  </div>
</template>

<script>
export default {
  name: "home"
};
</script>
 <style lang="scss" scoped>
.home {
  width: 100%;
  height: 100%;
  display: flex;
  flex-direction: column;
}
.header {
  width: 100%;
  height: 100px;
  background: #000;
  color: #fff;
}
.main {
  flex: 1;
  .van-swipe {
    width: 100%;
    height: 200px;
  }
  .van-swipe__track {
    height: 100%;
    width: 100%;
  }
  .van-swipe-item {
    height: 100%;
    width: 100%;
    background: hotpink;
  }
}
.footer {
  width: 100%;
  height: 60px;
  border-top: 1px solid #000;

  span {
    text-align: center;
    line-height: 60px;
    margin-left: 30px;
  }
}
</style>

