<template>
  <div id="homes">
    <div class="row">
      <div id="home" class="col-sm-12 text-center">
        <div class="background">
          <h2>欢迎大家品尝</h2>
          <h3>这里有你非常喜欢的pizza</h3>
          <button @click="gotoMenu" class="btn btn-success">Lets order</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'homes',
    methods: {
      gotoMenu() {
        // 跳转到上一级浏览页面
        // this.$router.go(-1)

        //  跳转到制定地址
        //   this.$router.replace('/menu')

        //  制定跳转路由名字
        //   this.$router.replace({name:'aboutLink'})

        //  通过push进行跳转
        // this.$router.push('/menu')
      }
    }
  }

</script>

<style scoped>
  #home{
    background: url('../../src/assets/pizza.jpg') no-repeat;
    height: 85vh;
    padding: 10%;
  }
  h2, h3{
    margin: 6%;
  }
  .background{
    background: #eee;
    opacity: 0.8;
    max-width: 70vw;
    margin: 0 auto;
    padding: 20px 0;
  }
</style>
