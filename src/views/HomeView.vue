<template>
  <div>
    <el-container>
      <el-header class="layout-header">
        <div class="login-user">
          <span class="welcome">欢迎回来，root!</span>
          <el-dropdown>
            <el-avatar src="https://cube.elemecdn.com/3/7c/3ea6beec64369c2642b92c6726f1epng.png"
                       size="small"></el-avatar>
            <el-dropdown-menu slot="dropdown">
              <el-dropdown-item icon="el-icon-plus">修改资料</el-dropdown-item>
              <el-dropdown-item icon="el-icon-circle-plus">修改头像</el-dropdown-item>
              <el-dropdown-item icon="el-icon-circle-plus-outline">修改密码</el-dropdown-item>
              <el-dropdown-item icon="el-icon-check" divided>退出登录</el-dropdown-item>
            </el-dropdown-menu>
          </el-dropdown>
        </div>
        <h1>酷鲨商城运营管理平台</h1>
      </el-header>
      <el-container class="layout-body">
        <el-aside class="layout-aside">
          <el-menu
              default-active="2"
              class="el-menu-vertical-demo"
              background-color="#545c64"
              text-color="#fff"
              active-text-color="#ffd04b"
              style="overflow: hidden">
<!--            首页-->
            <el-menu-item index="1">
              <i class="el-icon-menu"></i>
              <span slot="title">首页</span>
            </el-menu-item>
<!--            商品管理-->
            <el-submenu index="2">
              <template slot="title">
                <i class="el-icon-location"></i>
                <span>商品管理</span>
              </template>
              <el-menu-item index="2-1">
                <i class="el-icon-menu"></i>
                <span slot="title">SPU台账</span>
              </el-menu-item>
              <el-menu-item index="2-2">
                <i class="el-icon-menu"></i>
                <span slot="title">新增SPU</span>
              </el-menu-item>
              <el-menu-item index="2-3">
                <i class="el-icon-menu"></i>
                <span slot="title">相册管理</span>
              </el-menu-item>
              <el-menu-item index="2-4">
                <i class="el-icon-menu"></i>
                <span slot="title">商品类别</span>
              </el-menu-item>
              <el-menu-item index="2-5">
                <i class="el-icon-menu"></i>
                <span slot="title">属性模板</span>
              </el-menu-item>
              <el-menu-item index="2-6">
                <i class="el-icon-menu"></i>
                <span slot="title">属性管理</span>
              </el-menu-item>
              <el-menu-item index="2-7">
                <i class="el-icon-menu"></i>
                <span slot="title">品牌管理</span>
              </el-menu-item>
            </el-submenu>
<!--            订单管理-->
            <el-submenu index="3">
              <tmplate slot="title">
                <i class="el-icon-location"></i>
                <span>订单管理</span>
              </tmplate>
              <el-menu-item index="3-1">
                <i class="el-icon-menu"></i>
                <span slot="title">订单列表</span>
              </el-menu-item>
            </el-submenu>
          </el-menu>
        </el-aside>
        <el-main class="layout-main">
          这是底部主体
        </el-main>
      </el-container>
    </el-container>
  </div>
</template>
<style>
.layout-header {
  background-color: #409EFF;

}
.layout-header h1 {
  line-height: 30px;
  color: #fff;
}
.layout-header .login-user {
  float: right;
  display: flex;
  margin-top: 16px;
}
.layout-header .login-user .welcome {
  line-height: 10px;
  color: #fff;
  margin-top: 10px;
  margin-right: 20px;
}
.layout-body {
  border: 10px solid #000;
}
.layout-aside {
  background-color: #545c64;
  color: #fff;
  text-align: center;
  line-height: 200px;

}
.layout-main {
  background-color: #ebeef5;
  color: #333;
  text-align: center;
  line-height: 160px;
}
</style>
