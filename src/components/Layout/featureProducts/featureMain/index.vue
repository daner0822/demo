<template>
  <ul>
    <li>
      <div class="img_info">img</div>
      <div class="content">
        <div class="title line-clamp2">
          试真的试真的试真的试真的试真的试真的试真的试真的试真的试真的试真的真的试真的试真的真的试真的试真的
        </div>
        <div class="info">品质出游, 质量保证</div>
        <div class="detail">
          <div class="left line-clamp1">12月14日宜昌出发</div>
          <div class="right">￥1900起</div>
        </div>
      </div>
    </li>
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
    <li>aaa</li>
  </ul>
</template>

<script>
export default {
  data() {
    return {};
  }
};
</script>

<style lang="scss" scoped>
.line-clamp2 {
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
}
.line-clamp1 {
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  -webkit-line-clamp: 1;
  -webkit-box-orient: vertical;
}
ul {
  // width: 1200px;
  display: flex;
  flex-wrap: wrap;
  li {
    list-style: none;
    display: inline-block;
    width: 282px;
    height: 262px;
    box-sizing: border-box;
    border: 1px solid #000;
    margin-right: 24px;
    margin-bottom: 20px;
    &:nth-child(4n) {
      margin-right: 0;
    }
    .img_info {
      height: 138px;
      line-height: 138px;
      text-align: center;
      font-size: 25px;
      font-weight: 700px;
    }
    .content {
      padding: 10px;
      .title {
        font-size: 16px;
        color: #333333;
        text-align: left;
      }
    }
    .info {
      font-size: 12px;
      color: #999999;
      margin: 10px 0;
      text-align: left;
    }
    .detail {
      display: flex;
      justify-content: space-between;
      align-items: center;
      .left {
        width: 100px;
        height: 14px;
        font-size: 12px;
      }
      .right {
        font-size: 18px;
        color: #ba0d23;
      }
    }
  }
}
</style>
