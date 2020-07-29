<style scoped>
.layout {
  border: 1px solid #d7dde4;
  background: #f5f7f9;
  position: relative;
  border-radius: 4px;
  overflow: hidden;
  height: 100vh;
}
.layout-header-bar {
  background: #fff;
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.1);
}

.ivu-layout-sider,
.ivu-menu-dark.ivu-menu-vertical .ivu-menu-opened,
.ivu-menu {
  background: #191a23;
}
.layout-logo-left {
  width: 90%;
  height: 30px;
  border-radius: 3px;
  background: #191a23;
  margin: 15px auto;
}
.ivu-menu-dark {
  background: #191a23;
}
.menu-icon {
  transition: all 0.3s;
}
.rotate-icon {
  transform: rotate(-90deg);
}
.menu-item span {
  display: inline-block;
  overflow: hidden;
  width: 69px;
  text-overflow: ellipsis;
  white-space: nowrap;
  vertical-align: bottom;
  transition: width 0.2s ease 0.2s;
}
.menu-item i {
  transform: translateX(0px);
  transition: font-size 0.2s ease, transform 0.2s ease;
  vertical-align: middle;
  font-size: 16px;
}
.collapsed-menu span {
  width: 0px;
  transition: width 0.2s ease;
}
.collapsed-menu i {
  transform: translateX(5px);
  transition: font-size 0.2s ease 0.2s, transform 0.2s ease 0.2s;
  vertical-align: middle;
  font-size: 22px;
}

.logo {
  width: 100%;
}
.logo img {
  width: 80%;
}
.ivu-layout.ivu-layout-has-sider,
.ivu-layout-sider {
  height: 100%;
}
.layout-header-bar[data-v-81f9014e] {
  text-align: left;
}
.left {
  float: left;
  display: flex;
  height: 100%;
  align-items: center;
}
.right {
  float: right;
  height: 100%;
  display: flex;
  align-items: center;
}
.right ul {
  list-style: none;
  display: flex;
  align-items: center;
}
.right ul li {
  margin: 0 5px;
}
.ivu-badge {
  height: 30px;
}
.ivu-layout-header {
  line-height: 30px;
}
.right .ivu-badge-count {
  width: 10px;
  height: 10px;
}
.contentTitle {
  width: 100%;
  background-color: #fff;
  text-align: left;
  box-sizing: border-box;
  padding: 20px;
  margin-bottom: 20px;
}
.contentTitle h2,
.contentTitle p {
  font-weight: lighter;
  margin: 10px 0;
}
.table {
  background-color: #fff;
}
.table input {
  width: 100%;
}
.ivu-col-span-lg-8 {
  text-align: left;
}
</style>
<template>
  <div class="layout">
    <Layout>
      <Sider
        breakpoint="md"
        ref="side1"
        hide-trigger
        collapsible
        :collapsed-width="78"
        v-model="isCollapsed"
        width="256px"
      >
        <div class="logo">
          <img src="../../assets/img/logo-dark.ab519d9f.png" alt />
        </div>
        <Menu theme="dark" width="auto" :class="menuitemClasses" accordion>
          <Submenu name="1">
            <template slot="title">
              <Icon type="ios-paper" />内容管理
            </template>
            <MenuItem name="1-1">文章管理</MenuItem>
            <MenuItem name="1-2">评论管理</MenuItem>
            <MenuItem name="1-3">举报管理</MenuItem>
          </Submenu>
          <Submenu name="2">
            <template slot="title">
              <Icon type="ios-people" />用户管理
            </template>
            <MenuItem name="2-1">新增用户</MenuItem>
            <MenuItem name="2-2">活跃用户</MenuItem>
          </Submenu>
          <Submenu name="3">
            <template slot="title">
              <Icon type="ios-stats" />统计分析
            </template>
            <MenuGroup title="使用">
              <MenuItem name="3-1">新增和启动</MenuItem>
              <MenuItem name="3-2">活跃分析</MenuItem>
              <MenuItem name="3-3">时段分析</MenuItem>
            </MenuGroup>
            <MenuGroup title="留存">
              <MenuItem name="3-4">用户留存</MenuItem>
              <MenuItem name="3-5">流失用户</MenuItem>
            </MenuGroup>
          </Submenu>
          <Submenu name="4">
            <template slot="title">
              <Icon type="ios-stats" />详情页面
            </template>
            <MenuItem name="4-1">新增和启动</MenuItem>
            <MenuItem name="4-2">活跃分析</MenuItem>
            <MenuItem name="4-3">时段分析</MenuItem>
            <MenuItem name="4-4">用户留存</MenuItem>
            <MenuItem name="4-5">流失用户</MenuItem>
          </Submenu>
          <Submenu name="5">
            <template slot="title">
              <Icon type="ios-stats" />结果页面
            </template>
            <MenuGroup title="使用">
              <MenuItem name="5-1">新增和启动</MenuItem>
              <MenuItem name="5-2">活跃分析</MenuItem>
              <MenuItem name="5-3">时段分析</MenuItem>
            </MenuGroup>
            <MenuGroup title="留存">
              <MenuItem name="5-4">用户留存</MenuItem>
              <MenuItem name="5-5">流失用户</MenuItem>
            </MenuGroup>
          </Submenu>
          <Submenu name="6">
            <template slot="title">
              <Icon type="ios-paper" />列表页面
            </template>
            <MenuItem name="6-1">基础列表</MenuItem>
            <MenuItem name="6-2">卡片列表</MenuItem>
            <MenuItem name="6-3">查询表格</MenuItem>
          </Submenu>
        </Menu>
      </Sider>

      <Layout>
        <Header :style="{padding: 0}" class="layout-header-bar">
          <div class="left">
            <Icon
              @click.native="collapsedSider"
              :class="rotateIcon"
              :style="{margin: '0 20px'}"
              type="md-menu"
              size="24"
            ></Icon>
            <Row>
              <Col :xs="0" :md="24">
                <Breadcrumb>
                  <BreadcrumbItem>首页</BreadcrumbItem>
                  <BreadcrumbItem>列表页面</BreadcrumbItem>
                  <BreadcrumbItem>查询列表</BreadcrumbItem>
                </Breadcrumb>
              </Col>
            </Row>
          </div>
          <div class="right">
            <ul>
              <li>
                <Row>
                  <Col :xs="0" :lg="24">
                    <Input v-model="value" placeholder="搜索..." style="width: 230px" />
                  </Col>
                  <Col :xs="24" :lg="0">
                    <Icon type="ios-search-outline" size="24" />
                  </Col>
                </Row>
              </li>
              <li>
                <Icon type="md-radio-button-on" size="24" />
              </li>
              <li>
                <Icon type="md-qr-scanner" size="24" />
              </li>
              <li>
                <Badge :count="3" size="12">
                  <Icon type="ios-notifications-outline" size="26"></Icon>
                </Badge>
              </li>
              <li>
                <div>
                  <img src alt />
                  Aresn
                </div>
              </li>
              <li>
                <Icon type="md-football" size="24" />
              </li>
              <li>
                <Icon type="md-more" @click="value1 = true" size="24" />
              </li>
              <li>
                <Drawer title="Basic Drawer" :closable="false" v-model="value1">
                  <p>Some contents...</p>
                  <p>Some contents...</p>
                  <p>Some contents...</p>
                </Drawer>
              </li>
            </ul>
          </div>
        </Header>
        <Content :style="{margin: '20px', background: '#eee', minHeight: '260px'}">
          <div class="contentTitle">
            <h2>查询表格</h2>
            <p>表格查询的复杂示例</p>
          </div>
          <div class="table">
            <Row>
              <Col :xs="24" :lg="8">
                <label>规则名称：</label>
                <Input v-model="value" placeholder="搜索..." style="width:80%" />
              </Col>
              <Col :xs="24" :lg="8">
                <label>使用状态：</label>
                <Input v-model="value" placeholder="搜索..." style="width:80%" />
              </Col>
              <Col :xs="24" :lg="8">
                <Button type="primary">Primary</Button>
                <Button type="primary">Primary</Button>
                <Button type="primary">Primary</Button>
              </Col>
            </Row>
            <Table border :columns="columns7" :data="data6"></Table>
          </div>
        </Content>
      </Layout>
    </Layout>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isCollapsed: false,
      value: "",
      value1: false,
      columns7: [
        {
          title: "Name",
          key: "name",
          render: (h, params) => {
            return h("div", [
              h("Icon", {
                props: {
                  type: "person",
                },
              }),
              h("strong", params.row.name),
            ]);
          },
        },
        {
          title: "Age",
          key: "age",
        },
        {
          title: "Address",
          key: "address",
        },
        {
          title: "Action",
          key: "action",
          width: 150,
          align: "center",
          render: (h, params) => {
            return h("div", [
              h(
                "Button",
                {
                  props: {
                    type: "primary",
                    size: "small",
                  },
                  style: {
                    marginRight: "5px",
                  },
                  on: {
                    click: () => {
                      this.show(params.index);
                    },
                  },
                },
                "View"
              ),
              h(
                "Button",
                {
                  props: {
                    type: "error",
                    size: "small",
                  },
                  on: {
                    click: () => {
                      this.remove(params.index);
                    },
                  },
                },
                "Delete"
              ),
            ]);
          },
        },
      ],
      data6: [
        {
          name: "John Brown",
          age: 18,
          address: "New York No. 1 Lake Park",
        },
        {
          name: "Jim Green",
          age: 24,
          address: "London No. 1 Lake Park",
        },
        {
          name: "Joe Black",
          age: 30,
          address: "Sydney No. 1 Lake Park",
        },
        {
          name: "Jon Snow",
          age: 26,
          address: "Ottawa No. 2 Lake Park",
        },
      ],
    };
  },
  computed: {
    rotateIcon() {
      return ["menu-icon", this.isCollapsed ? "rotate-icon" : ""];
    },
    menuitemClasses() {
      return ["menu-item", this.isCollapsed ? "collapsed-menu" : ""];
    },
  },
  methods: {
    collapsedSider() {
      this.$refs.side1.toggleCollapse();
    },
    show(index) {
      this.$Modal.info({
        title: "User Info",
        content: `Name：${this.data6[index].name}<br>Age：${this.data6[index].age}<br>Address：${this.data6[index].address}`,
      });
    },
    remove(index) {
      this.data6.splice(index, 1);
    },
  },
};
</script>
