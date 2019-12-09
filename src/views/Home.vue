<template>
  <div class="home">
    <!-- 导航 -->
    <nav class="nav">
      <div class="nav_container">
        <span>logo</span>
        <ul class="nav_container__list">
          <li>首页</li>
          <li>发现</li>
        </ul>
      </div>
    </nav>
    <!-- 需要被隐藏的模块 -->
    <section class="section">
      <div class="section_container">
        <div>
          <span>logo</span>
          <div class="section_container__text">
            <h3>welcome</h3>
            <p>The block of content passed to a mixin are evaluated in the scope where the block is defined, not in the scope of the mixin. This means that variables local to the mixin cannot be used within the passed style block and variables will resolve to the global value:</p>
          </div>
        </div>
        <div class="section_container__title">
          <span class="section_container__title__num">
            <span>感谢您已成为第</span>
            <h3>09</h3>
            <span>位访客大大~</span>
          </span>
          <p class="section_container__title__btn"> <span><<</span> 开启属于自己的初体验 <span>>></span> </p>
        </div>
      </div>
    </section>
    <!-- 主体模块 -->
    <main></main>
    <!-- <div class="box">99999</div>
    <div class="foot">111111</div>-->
  </div>
</template>

<script>
export default {
  name: "home",
  data() {
    return {};
  }
};
</script>
<style lang="scss" scoped>
// 颜色
$tetxColor: rgba(75, 140, 120, 1);
// 复用样式
.content {
  max-width: 1360px;
  margin: auto;
}
.home {
  font-family: "zz-Light";
  position: relative;
  .nav {
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    border-bottom: 1px solid #ebebeb;
    background-color: rgba(255, 255, 255, 0.9);
    &_container {
      @extend .content;
      padding: 0 15px;
      display: flex;
      align-items: center;
      height: 55px;
      &__list {
        font-size: 13px;
        margin: 0 0 0 40px;
        display: flex;
        li {
          padding-top: 5px;
          margin: 0 20px;
          &:hover {
            color: #999;
          }
        }
      }
    }
  }
  .section {
    width: 100%;
    position: absolute;
    left: 0px;
    top: 56px;
    line-height: 20px;
    text-align: center;
    // background-color: pink;
    &_container {
      @extend .content;
      padding: 40px 0;
      color: $tetxColor;
      &__text {
        padding: 30px 0;
        font-size: 20px;
        p {
          margin: 0 auto;
          padding-top: 40px;
          width: 50%;
          font-size: 12px;
          line-height: 24px;
        }
      }
      &__title {
        margin-top: 10%;
        &__num {
          justify-content: center;
          display: flex;
          span {
            padding: 0 3%;
            font-size: 24px;
          }
          h3 {
            font-size: 90px;
            font-weight: 600;
          }
        }
        &__btn {
          font-size: 16px;
          margin: 8% -2% 0 0;
          span {
            font-size: 12px;
            padding: 0 2%;
          }
        }
      }
    }
  }
}
</style>
