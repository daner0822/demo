<template>
  <div class="header">
    <div class="header_logo container">
      <div class="logo">
      <img src="../../assets/logo.png" alt=""/>
      </div>
        <ul class="service">
          <li>
            <img src="../../assets/price_guarantee.png" alt="">
            <p>价格保证</p> 
            </li>
          <li>
            <img src="../../assets/security.png" alt="">
            <p>安全保障</p>
          </li>
          <li>
            <img src="../../assets/Unsub_protection.png" alt="">
            <p>退订保障</p>
          </li>
          <li>
            <img src="../../assets/service.png" alt="">
            <p>24h服务</p>
            </li>
        </ul>
    </div>
    <div class="header-top">
      <div class="container nav">
      <div class="nav_left">
        <ul>
          <li>
            <img src="../../assets/index.png" alt="">
            <span>首页</span>
            </li>
             <li>
            <img src="../../assets/proList.png" alt="">
            <span>产品列表</span>
            </li> <li>
            <img src="../../assets/proBooking.png" alt="">
            <span>产品预订</span>
            </li>
        </ul>
      </div>
        <!-- 登录｜注册 -->
      <div class="nav_right">
        <a href="#">登录｜</a>
        <a href="#">注册</a>
      </div>
      </div>
      <div>
      </div>
    
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
@import "@/assets/scss/index.scss";
.header{
  background-color: #fff;
  .header_logo{
    display: flex;
    justify-content: space-between;
    .logo{
      margin-top: 15px;
    }
    .service{
      li{
        float: left;
        img{
          display: block;
          margin-top: 10px;
          margin-left: 32px;
        }
        p{
          text-align: center;
          font-size: 14px;
          color: #666;
          margin: 5px 0;
          margin-left: 16px;
        }
      }
    }
  }
  .header-top{
    // width:100%;
  height: 40px;
  background-color: $bg-color;
  .nav{
    display: flex;
    justify-content:  space-between;
    .nav_left{
      li{
        float: left;
        width: 220px;
        text-align: left;
        line-height: 40px;
        img{
          vertical-align:middle
        }
        span{
          color: #fff;
          font-size: 16px;
          margin-left: 10px;
          vertical-align:middle
        }
      }
    }
    .nav_right{
      a{
        color: #fff;
        font-size: 16px;
        line-height: 40px;
      }
    }
  }

  }
}
</style>