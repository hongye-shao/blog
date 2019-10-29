<template>

  <Layout>
   <Navbar></Navbar>
   <Content>
   <Row type="flex" :gutter="10" justify="center" style="margin-top:10px;">
    <Col  span="11" :xs="24" :sm="24" :md="11" :lg="11">
      <div class="layout-left">
        <div class="recommend-index">
          <div class="recommentd-top">
           <Carousel>
              <CarouselItem>
              <img class="d-block" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/12.jpg" />
              </CarouselItem>
              <CarouselItem>
              <img class="d-block" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/13.jpg" />
              </CarouselItem>
            </Carousel>
          </div>
          <div class="recommentd-bottom">
            <div class="recommentd-item">
              <img  class="img-fluid" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/16.jpg"/>
            </div>
            <div class="recommentd-item">
              <img  class="img-fluid" src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/21.jpg"/>
            </div>  
          </div>
        </div>
        <List>
          
        <ListItem>
          <template slot="extra">
                <img src="https://dev-file.iviewui.com/5wxHCQMUyrauMCGSVEYVxHR5JmvS7DpH/large" style="width: 280px">
            </template>
            <ListItemMeta  title="This is title" description="This is description, this is description." />
        </ListItem>
        <ListItem>
          <template slot="extra">
                <img src="https://dev-file.iviewui.com/5wxHCQMUyrauMCGSVEYVxHR5JmvS7DpH/large" style="width: 280px">
            </template>
            <ListItemMeta  title="This is title" description="This is description, this is description." />
        </ListItem>
       
    </List>
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

.layout-right {
  background: blue;
}
.recommentd-top{
  margin-bottom: 20px;
}
.recommentd-bottom {
  display: flex;
  justify-content: space-between;
}
.recommentd-item{
      width: 49%;
      height: 170px;
      overflow: hidden;
}
.d-block{
  width: 100%;
}
.img-fluid{
  width: 100%;
  height: auto;
}
</style>
