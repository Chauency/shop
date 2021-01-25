<template>
  <div class="login_container">
    <div class="login_box">
      <!--头像区域-->
      <div class="avatar_box">
        <img src="../assets/logo.png" alt="">
      </div>
      <!--登录表单区域-->
      <el-form ref="form" label-width="80px">
        <el-form-item label="活动名称">
          <el-input></el-input>
        </el-form-item>
      </el-form>

    </div>
  </div>
</template>

<script>
export default {
  name: "Login"
}
</script>

<style lang="less" scoped>
.login_container {
  background-color: #2b4b6b;
  height: 100%;
}

.login_box {
  width: 450px;
  height: 300px;
  background-color: #fff;
  /*以下四句是的box全屏居中*/
  position: absolute; /*绝对位置*/
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);

  /*less 语法嵌套*/

  .avatar_box {
    height: 130px;
    width: 130px;
    border: 1px solid #eee; /*边框*/
    border-radius: 50%; /*圆形边框*/
    padding: 10px;
    box-shadow: 0 0 10px #ddd;

    position: absolute;
    left: 50%;
    transform: translate(-50%, -50%);

    background-color: #fff;

    img {
      width: 100%;
      height: 100%;
      background-color: #eee;
      border-radius: 50%;

    }

  }
}
</style>