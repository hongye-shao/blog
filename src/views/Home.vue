<template>
  <Layout>
    <Navbar></Navbar>
    <Content>
      <Row type="flex" :gutter="10" justify="center" style="margin-top:10px;">
        <Col  :xs="24" :sm="24" :md="10" :lg="10">
          <div class="layout-left">
            <div class="recommend-index">
              <div class="recommentd-top">
                <Carousel>
                  <CarouselItem>
                    <img
                      class="d-block"
                      src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/12.jpg"
                    />
                  </CarouselItem>
                  <CarouselItem>
                    <img
                      class="d-block"
                      src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/13.jpg"
                    />
                  </CarouselItem>
                </Carousel>
              </div>
              <div class="recommentd-bottom">
                <div class="recommentd-item">
                  <img
                    class="img-fluid"
                    src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/16.jpg"
                  />
                </div>
                <div class="recommentd-item">
                  <img
                    class="img-fluid"
                    src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/21.jpg"
                  />
                </div>
              </div>
            </div>
           <Card shadow style="margin: 0 0 20px 0;">
             <Row  type="flex" :gutter="10"  >
               <Col :sm="24" :md="4" :lg="6" class-name="cl-card-image">
               <img class="img-fluid" src="https://cdn.fastadmin.net/uploads/20180507/d197f62611ff69b738e114add9f3183b.jpg"/>
               </Col>
                <Col :sm="12" :md="8" :lg="18" class-name="cl-card-main">
                  <h3 class="cl-card-main-title">博客的时代正在到来</h3>
                  <div class="cl-card-main-info">
                    <p>全世界每天传播的媒体内容，有一半是由6大媒体巨头所控制。其利益驱动、意识形态以及传统的审查制度，使得这些经过严重加工处理的内容已经越来越不适应人们的需求。媒体的工业化，内容出口的工厂化，都在严重影响其发展。<br>比如，以美联社为例，有近4000人专业记者，每天“制造并出厂”2000万字的内容，每天发布在8500多种报纸、杂志和广播中，把读者当作“信息动物”一样。这种大教堂式的模式主导了整个媒体世界。这时，以个人为中心的博客潮流却开始有力冲击传统媒体，尤其是对新闻界多年形成的传统观念和道德规范。</p>
                  </div>

               </Col>
             </Row>
           </Card>

            <Card shadow style="margin: 0 0 20px 0;">
              <Row  type="flex" :gutter="10"  >
                <Col :sm="24" :md="4" :lg="6" class-name="cl-card-image">
                <img class="img-fluid" src="https://cdn.fastadmin.net/uploads/20180507/d197f62611ff69b738e114add9f3183b.jpg"/>
                </Col>
                <Col :sm="12" :md="8" :lg="18" class-name="cl-card-main">
                <h3 class="cl-card-main-title">博客的时代正在到来</h3>
                <div class="cl-card-main-info">
                <p>全世界每天传播的媒体内容，有一半是由6大媒体巨头所控制。其利益驱动、意识形态以及传统的审查制度，使得这些经过严重加工处理的内容已经越来越不适应人们的需求。媒体的工业化，内容出口的工厂化，都在严重影响其发展。<br>比如，以美联社为例，有近4000人专业记者，每天“制造并出厂”2000万字的内容，每天发布在8500多种报纸、杂志和广播中，把读者当作“信息动物”一样。这种大教堂式的模式主导了整个媒体世界。这时，以个人为中心的博客潮流却开始有力冲击传统媒体，尤其是对新闻界多年形成的传统观念和道德规范。</p>
                </div>
                </Col>
              </Row>
            </Card>


          </div>
        </Col>

        <Col  :xs="15" :sm="15" :md="3" :lg="3">
          <div class="layout-right">右边内容</div>
        </Col>
      </Row>
    </Content>
    <Footer
      style="background:#ffff; margin-top:50px"
    >Copyright @ 2017~2019 Theme design by jeanstudio</Footer>
  </Layout>
</template>

<script>
// @ is an alias to /src
import Navbar from "@/components/Navbar.vue";
export default {
  name: "home",
  data() {
    return {};
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
.recommentd-top {
  margin-bottom: 20px;
}
.recommentd-bottom {
  display: flex;
  justify-content: space-between;
}
.recommentd-item {
  width: 49%;
  height: 170px;
  overflow: hidden;
}
.d-block {
  width: 100%;
}
.img-fluid {
  width: 100%;
  height: auto;
}
.ivu-card-body .cl-card-image{
  overflow: hidden;

}

.ivu-card-body .cl-card-image img{
 width: 100%;
 max-width: 100%;
}
.cl-card-main-title {
  height: 2rem;
  overflow: hidden;
  text-align: left;
}
.cl-card-main-info{
  font-size: 1rem;
  color: #999;
  height: 3rem;
  overflow: hidden;
  margin: 0.5rem 0 2rem 0;
  text-align: justify;
}
</style>
