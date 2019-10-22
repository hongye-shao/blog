<template>
 <div class="navbar">
   <Header>
      <div class="navbar-header">
     <Row>
       <Col :lg="24" :md="24" :sm="0" :xs="0">
        <Menu mode="horizontal" theme="light" active-name="1">
                    <div class="layout-logo">
                      logo
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
                </Menu>
       </Col>
       <Col :lg="0" :md="0" :sm="24" :xs="24">
       
       </Col>
     </Row>
   </div>
   </Header>
 </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'home',

}
</script>
<style scoped>
.ivu-layout-header {
  background:#ffff;
  height: 80.75px;
}
 .ivu-menu {
  background:#ffffff;
  max-width: 1140px;
  margin: auto;
   height: 80.75px;
}
.layout-logo{
  background: red;
  width: 100px;
  height: 30px;
  float: left;
  position: relative;
  top: 15px;
  left: 20px;
}
.layout-nav{
    width: 420px;
    margin: 0 auto;
    margin-right: 20px;
}

</style>
