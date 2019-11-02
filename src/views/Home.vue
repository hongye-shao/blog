<template>
  <Layout>
    <Navbar></Navbar>
    <Content>
      <Row type="flex" :gutter="10" justify="center" style="margin-top:10px;">
        <Col :xs="24" :sm="24" :md="10" :lg="10">
          <div class="layout-left">
            <Index></Index>
          </div>
        </Col>

        <Col :xs="22" :sm="22" :md="3" :lg="3">
          <div class="layout-right">
            <Card shadow class="right-card">
              <div class="right-card-title">这里是标题</div>
              <div class="cl-code">
                <img class="img-fluid" src="@/assets/544.jpg" />
              </div>
            </Card>

            <Card shadow class="right-card">
              <div class="right-card-title">最新文章</div>
              <List>
                <ListItem>
                  <Icon type="ios-arrow-forward" />This is a piece of text.
                </ListItem>
                <ListItem>
                  <Icon type="ios-arrow-forward" />This is a piece of text.
                </ListItem>
                <ListItem>
                  <Icon type="ios-arrow-forward" />This is a piece of text.
                </ListItem>
                <ListItem>
                  <Icon type="ios-arrow-forward" />This is a piece of text.
                </ListItem>
              </List>
            </Card>
            <!-- <Card :padding="0" :bordered="false" :dis-hover="true" style=" background: red;">
              <img
                src="https://cdn.demo.fastadmin.net/assets/addons/blog/default/example/12.jpg"
                style="width:100%"
              />
            </Card> -->
          </div>
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
import Index from "@/components/Index.vue";
export default {
  name: "home",
  data() {
    return {};
  },
  components: {
    Navbar,
    Index
  }
};
</script>
<style scoped>
.right-card-title {
 
  font-size: 1.2rem;
  color: #666;
  font-weight: bold;
  text-align: left;
}
.cl-code {
  width: 80%;
  margin: 10px auto;
  padding: 0 0 10px 0;
}
.img-fluid {
  max-width: 100%;
  height: auto;
}
.right-card {
  margin-bottom: 20px;
}
</style>
