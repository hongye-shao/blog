<template>

  <Layout>
   <Navbar></Navbar>
   <Content>
   <Row type="flex" :gutter="10" justify="center">
        <Col  span="11" :xs="24" :sm="24" :md="11" :lg="11">
        <div class="layout-left">
           左边内容
        </div>
        </Col>

        <Col  span="4" :xs="15" :sm="15" :md="4" :lg="4" >
        <div class="layout-right">
           右边内容
        </div>

        </Col>

      </Row> 
   </Content>
   <Footer style="background:#ffff; margin-top:50px" >
     Copyright @ 2017~2019 Theme design by jeanstudio
     </Footer>
  </Layout>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
export default {
  name: "home",
  data() {
    return {

    };
  },
  components: {
    Navbar
  }
};
</script>
<style scoped>

.layout-left {
  background: red;
}
.layout-right {
  background: blue;
}
</style>
