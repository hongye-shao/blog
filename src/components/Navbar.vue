<template>
   <Row>
       <Col :lg="24" :md="24" :sm="0" :xs="0">
          <Menu mode="horizontal" theme="light" active-name="1">
            <div class="navbar">
              <div class="logo">
                <!-- <img class="logo-img" src="@/assets/544.jpg" > -->
                这里是LOG
              </div>
              <div class="layout-nav">
                <MenuItem name="1">
                  <Icon type="ios-navigate"></Icon>
                  首页
                </MenuItem>
                <MenuItem name="2">
                  <Icon type="ios-keypad"></Icon>
                  归档
                </MenuItem>
                <MenuItem name="3">
                  <Icon type="ios-analytics"></Icon>
                  关于我
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
                  <Icon @click="toggleMobileMenu" type="ios-menu" size="45" style="margin-top:8px" color="#000"/>
               </div>
          </div>
        <Drawer  placement="left" :closable="false" v-model="showMobileMenu">
           <Menu theme="light" active-name="1">
          <MenuGroup>
            <MenuItem name="1">
                <Icon type="md-document" />
               首页
            </MenuItem>
            <MenuItem name="2">
                <Icon type="md-chatbubbles" />
               归档
            </MenuItem>
             <MenuItem name="2">
                <Icon type="md-chatbubbles" />
                关于我
            </MenuItem>
          </MenuGroup>
        </Menu>
        </Drawer>
       </Col>
     </Row>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'navbar',
  data()  {
    return {
        showMobileMenu : false
    }
  },
  mounted(){
     window.onreset = () =>{
       if(window.innerWidth >= 768){
         this.showMobileMenu = false
       }
     }
  },
  methods: {
    toggleMobileMenu(){
      this.showMobileMenu = !this.showMobileMenu
    
    }
  }

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

  width: 210px;
  height: 72px;
  float: left;
  position: relative;
  top: 5px;
  left: 47px;
}
.logo .logo-img {
    width: 210px;
    height: 72px;
  }
.layout-nav{
    width: 314px;
    margin: 0 auto;
    margin-right: 20px;
}
.navbar-menu{
  width: 100%;
  height: 80.75px;
  background: #FFFFFF;
}
.layout-nav-sm .ivu-icon{
  font-size: 45px;
    color: rgb(0, 0, 0);
    position: relative;
    left: 49px;
    top: 14px;
}
.ivu-btn-icon-only.ivu-btn-large{
  width: 49.25px;
  height: 35.25px;
}

</style>
