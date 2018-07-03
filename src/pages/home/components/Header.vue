<template>
  <div class="header">
    <div class="header-left">
      <div class="iconfont back-icon">&#xe624;</div>
    </div>
    <div class="header-input">
      <span class="iconfont">&#xe632;</span>
      输入城市景点/游玩/主题
      </div>
    <div class="header-right">
      城市
      <span class="iconfont arrow-icon">&#xe62d;</span>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header'
}
</script>

<style lang="scss">
    @import '~styles/common.scss';
    .header{
      display: flex;
      background-color: $bgColor;
      color: #fff;
      line-height: .86rem;
      .header-left{
        width: .64rem;
        float: left;
        .back-icon{
          text-align: center;
          font-size: .4rem;
        }
      }
      .header-input{
        flex: 1;
        line-height: .64rem;
        height: .64rem;
        background-color: #fff;
        border-radius: .1rem;
        margin-top: .12rem;
        margin-left:.2rem;
        color: #cccccc;
        padding-left: .1rem
      }
      .header-right{
        width: 1.24rem;
        float: right;
        text-align: center;
        .arrow-icon{
          font-size: .24rem;
          margin-left: -.05rem;
        }
      }
    }
</style>
