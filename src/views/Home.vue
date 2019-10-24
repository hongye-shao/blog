<template>
   <Row>
       <Col :lg="24" :md="24" :sm="0" :xs="0">
          <Menu mode="horizontal" theme="light" active-name="1">
            <div class="navbar">
              <div class="logo">
                <img class="logo-img" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/img/logo.jpg">
              </div>
              <div class="layout-nav">
                <MenuItem name="1">
                  <Icon type="ios-navigate"></Icon>
                  Item 1
                </MenuItem>
                <MenuItem name="2">
                  <Icon type="ios-keypad"></Icon>
                  Item 2
                </MenuItem>
                <MenuItem name="3">
                  <Icon type="ios-analytics"></Icon>
                  Item 3
                </MenuItem>
                <MenuItem name="4">
                  <Icon type="ios-paper"></Icon>
                  Item 4
                </MenuItem>
              </div>
            </div>
          </Menu>
       </Col>
       <Col :lg="0" :md="0" :sm="24" :xs="24">
          <div class="navbar-menu">
               <div class="logo">
                <img class="logo-img" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/img/logo.jpg">
              </div>
               <div class="layout-nav-sm">
                  <Icon  type="ios-menu" size="45" style="margin-top:8px" color="#000"/>
               </div>
          </div>
        <Menu theme="light" active-name="1">
          <MenuGroup>
            <MenuItem name="1">
                <Icon type="md-document" />
                文章管理
            </MenuItem>
            <MenuItem name="2">
                <Icon type="md-chatbubbles" />
                评论管理
            </MenuItem>
             <MenuItem name="2">
                <Icon type="md-chatbubbles" />
                评论管理
            </MenuItem>
          </MenuGroup>
        </Menu>
       </Col>
     </Row>
 </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',

}
</script>
<style scoped>

.ivu-menu{
  height: 80.75px;
}
 .navbar {
  max-width: 1140px;
  margin: auto;
}
.logo{
  background: red;
  width: 210px;
  height: 72px;
  float: left;
  position: relative;
  top: 5px;
  left: 20px;
}
.logo .logo-img {
    width: 210px;
    height: 72px;
  }
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}
.navbar-menu{
  width: 100%;
  background: yellow;
  height: 80.75px;
}
.layout-nav-sm {
      position: relative;
      left: 54px;
      top: 22px;
}
.ivu-btn-icon-only.ivu-btn-large{
  width: 49.25px;
  height: 35.25px;
}

</style>
