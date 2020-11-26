<template>
  <div class="main-content">
      <div class="banner">
        <div class="container">
         <img src="../../assets/banner.jpg" alt="">
         <div class="search">
           <div class="search-info">
             <div class="left">
             <img src="../../assets/landmark.png" alt="">
             <span>上海</span>
             <i class="el-icon-arrow-down"></i>
             </div>
             <el-input placeholder="例如：邮轮、航线或目的地" class="search-input" v-model="input"></el-input>
             <div class="search-btn"> 搜索
             </div>
           </div>
         </div>
        </div>
      </div>
    <div class="product clearfix">
      <featureProducts></featureProducts>
    </div>
      <div class="cruise_comp">
          <div class="cruise_comp_title">
          <h1>邮轮公司</h1>
            <a class="more">
          <span>查看更多</span>
          <div class="icon">
          <i class="el-icon-arrow-right"></i>
          </div>
         </a>
          </div>
        <div class="container">
         <ul class="cruise_comp_list">
          <li></li>
          <li></li>
          <li></li>
          <li></li>
        </ul>
        </div>
      </div>
      <div></div>
  </div>
</template>

<script>
import featureProducts from "./featureProducts/index";

export default {
    components: {
    featureProducts
  },
  data(){
    return {
      input:''
    }
  }
}
</script>
<style lang="scss" scoped>
  @import "@/assets/scss/index.scss";
  .main-content{
    .banner{
      height: 150px;
      background-color: #fff;
      .container{
        display: flex;
        justify-content: space-between;
        .search{
          .search-info{
            display: flex;
            height: 46px;
            margin-top: 50px;
            margin-left: 150px;
            .left{
              border: 1px solid $bg-color;
              width: 220px;
              border-radius: 50px 0 0 50px;
              font-size: 16px;
              color: #333;
              img{
                vertical-align: middle;
                margin-left: -10px;
              }
              span{
                vertical-align: middle;
                line-height: 46px;
                margin-left: 5px;
              }
              i{
                vertical-align: middle;
                margin-left: 5px;
              }
            }
          .search-btn{
            color: #fff;
            width: 200px;
            font-size: 18px;
            height: 46px;
            line-height: 46px;
            border-radius: 0 25px 25px 0;
            background-color: $bg-color;
              border: 1px solid $bg-color;
          }
          .search-input{
            // width:60%;
            outline:none;
            // margin-left:105px;
              border: 1px solid $bg-color;
              border-left: none;;

          }
          }
        }
      }

    }
    .product{
      height: 560px;
      width: 1200px;
      margin: 0 auto;
      margin-bottom: 80px;
    }
     .cruise_comp{
      // height: 150px;
      .cruise_comp_title{
         display: flex;
        justify-content: space-between;
        max-width: 1200px;
        margin: 0 auto;
        margin-bottom: 10px;
          h1{
            font-size: 32px;
            color: #333;
          }
          .more{
            margin-top: 20px;
            font-size: 14px;

          }
          .icon{
            display: inline-block;
            width: 16px;
            height: 16px;
           line-height: 18px;
            background-color:$bg-color;
            border-radius: 50%;
            i{
              color: #fff;
            }
          }
        }
      .container{
        display: flex;
        justify-content: space-between;
        .cruise_comp_list{
          li{
          float: left;
          width: 298px;
          height: 360px;
          border: 1px solid $bg-color;
          }
        }
        
      }
    }
    /deep/ .el-input__inner {
      border:none !important;
      padding: 22px;
    }
  }
</style>