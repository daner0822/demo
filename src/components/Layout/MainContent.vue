<template>
  <div class="main-content">
      <div class="banner">
        <div class="container">
         <img src="../../assets/banner.jpg" alt="">
         <div class="search">
           <div class="search-text" >
             <div class="left">
             <img src="../../assets/landmark.png" alt="">
             <span>上海</span>
             <!-- <img src="../../assets/landmark.png" alt=""> -->
             </div>
             <!-- <button class="search_btn">搜索</button> -->
           </div>
         </div>
        </div>
      </div>
  </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  .main-content{
    height: 500px;
    overflow: hidden;
    .banner{
      height: 150px;
      background-color: #fff;
      .container{
        display: flex;
        justify-content: space-between;
        .search{
          .search-text{
            border: 1px solid #3971ff;
            width: 600px;
            height: 50px;
            border-radius: 25px;
            margin-top: 50px;
            position: relative;
            .left{
              position: absolute;
              top: 15px;
              left: 20px;
              img{
                vertical-align: middle;
              }
              span{
                vertical-align: middle;
                margin-left: 5px;
              }
            }
          .search_btn{
            outline: none;
            border: none;
          }
          }
        }
      }
    }
  }
</style>