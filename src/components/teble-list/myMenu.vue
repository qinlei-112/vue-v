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
.ivu-layout.ivu-layout-has-sider > .ivu-layout,
.ivu-layout.ivu-layout-has-sider > .ivu-layout-content {
  position: relative;
}
.layout-header-bar {
  position: absolute;
  top: 0;
  width: 100%;
  z-index: 10;
}
@media screen and (max-width: 730px) {
  .layout-header-bar {
    position: fixed;
  }
}
.ivu-row {
  box-sizing: border-box;
  padding: 20px 0;
}
.ivu-col-span-lg-8 {
  text-align: left;
  height: 100%;
  margin: 20px 0;
}
.ivu-col-span-lg-8:last-child {
  display: flex;
  align-items: center;
  justify-content: flex-end;
}
#primary {
  height: 100%;
  display: flex;
  align-items: center;
  box-sizing: border-box;
  padding: 0 10px;
}
#primary Button {
  margin: 0 10px;
}
#a {
  width: 100%;
  overflow: hidden;
}
#a Button {
  float: left;
}
.ivu-table-wrapper-with-border {
  width: 100%;
  min-width: 800px;
}
.footer {
  background: #eee;
}
.footer div {
  display: flex;
  align-items: center;
  justify-content: center;
}
.footer div p {
  margin-left: 10px;
}

.Monitor #img {
  width: 20px;
  height: 20px;
  border-radius: 100%;
  overflow: hidden;
}
.Monitor #img img {
  width: 100%;
}
.ivu-col-span-lg-6 {
  box-sizing: border-box;
  padding: 10px;
}
.col {
  width: 100%;
  height: 170px;
  background-color: #fff;
  padding: 10px;
}
.col Icon,
.col h2,
.col p,
.col div {
  margin: 10px 0;
}
.col h2 {
  font-size: 28px;
  color: #333;
}
.col p {
  color: #999;
}
.col .icon {
  width: 30px;
  height: 30px;
  background: rgba(123, 0, 0, 0.1);
  margin: 0 auto;
  border-radius: 100%;
  text-align: center;
  line-height: 30px;
}
.col div {
  font-weight: 600;
}
.Monitor .main .ivu-col-span-lg-16 {
  padding: 10px;
  box-sizing: border-box;
}
.Monitor .main .title {
  background-color: #fff;
  width: 100%;
  border-bottom: 1px solid #ccc;
  text-align: left;
  height: 50px;
  line-height: 50px;
}
.Monitor .centent h2{
  font-size: 40px;
}
.Monitor .centent {
  background-color: #fff;
  height: 160px;
  overflow: hidden;
}
.Monitor .centent h2,
.Monitor .centent i{
  margin: 10px 0;
}
.Monitor #main {
  width: 100%;
  background-color: #fff;
  padding: 10px;
  box-sizing: border-box;
}
.Monitor .footer {
  height: 180px;
  background-color: #fff;
  padding: 10px;
  box-sizing: border-box;
}
.Monitor .footer p {
  text-align: left;
}
.Monitor .footer > div {
  display: flex;
  justify-content: left;
}
.Monitor .footer h2 {
  font-size: 60px;
  font-weight: 100;
  text-align: left;
  margin-right: 20px;
}
.footer .top {
  height: 90px;
  border-bottom: 1px solid #ccc;
  display: flex;
}
.footer .top h2,
.footer .top>div {
  margin: 0;
  text-align: center;
}
.footer .top>div{
  flex:2;
  height: 100%;
}

.footer .top img {
  width: 40px;
  display: block;
}
.footer .top h2 {
  font-size: 28px;
  flex: 1;
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
              <Icon type="ios-paper" />Dashboard
            </template>
            <MenuItem name="1-1">主控台</MenuItem>
            <MenuItem name="1-2">
              <button
                @click="showMonitor()"
                style="border:0;outline: 0;background:transparent;color:#fff"
              >监控台</button>
            </MenuItem>
            <MenuItem name="1-3">工作台</MenuItem>
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
            <MenuItem name="6-3">
              <button
                @click="showFun()"
                style="border:0;outline: 0;background:transparent;color:#fff"
              >查询表格</button>
            </MenuItem>
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

        <Content
          :style="{margin: '20px', background: '#eee', minHeight: '260px',marginTop:'60px'}"
          v-show="showTable"
        >
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
                <div id="primary">
                  <Button type="primary" @click="loadingFun()">查询</Button>
                  <Button type="primary">重置</Button>
                  <Dropdown trigger="click" style="margin-left: 20px">
                    <a href="javascript:void(0)">
                      展开
                      <Icon type="ios-arrow-down"></Icon>
                    </a>
                    <DropdownMenu slot="list">
                      <DropdownItem>驴打滚</DropdownItem>
                      <DropdownItem>炸酱面</DropdownItem>
                      <DropdownItem>豆汁儿</DropdownItem>
                      <DropdownItem>冰糖葫芦</DropdownItem>
                      <DropdownItem>北京烤鸭</DropdownItem>
                    </DropdownMenu>
                  </Dropdown>
                </div>
              </Col>
            </Row>
            <div id="a">
              <Button type="primary">+ 新增</Button>
            </div>
            <Table
              border
              :columns="columns7"
              :data="data6"
              style="margin:30px 0"
              :loading="loading"
            ></Table>
            <Page :total="100" show-sizer style="margin-bottom:30px" />
          </div>

          <div class="footer">
            <div>
              <p>官网</p>
              <p>社区</p>
              <p>平台</p>
            </div>
            <div>
              <p>Copyright © 2019 北京视图更新科技有限公司</p>
            </div>
          </div>
        </Content>

        <Content
          :style="{margin: '20px', background: '#eee', minHeight: '260px',marginTop:'60px'}"
          v-show="flagMonitor"
        >
          <div class="Monitor">
            <div>
              <Row>
                <Col :xs="12" :lg="6" v-for="item in monitor" :key="item.icon">
                  <div class="col">
                    <div class="icon">
                      <Icon type="ios-analytics-outline" size="20" color="#f56" />
                    </div>
                    <h2>{{item.title}}</h2>
                    <p>{{item.text}}</p>
                    <div v-if="item.img" style="display:flex;justify-content: center;">
                      <div v-for="img in item.img" :key="img" id="img">
                        <img src="../../assets/img/avatar.png" alt />
                      </div>
                    </div>
                    <div v-if="item.click" style="color:green;">
                      <Icon type="ios-arrow-up" />
                      {{item.click}}
                    </div>
                    <div v-if="item.arrival" style="color:red">
                      <Icon type="ios-arrow-down" />
                      {{item.arrival}}
                    </div>
                    <div v-if="item.aransform" style="color:green">
                      <Icon type="ios-arrow-up" />
                      {{item.aransform}}
                    </div>
                  </div>
                </Col>
              </Row>
            </div>
            <div class="main">
              <Row>
                <Col :xs="24" :lg="18">
                  <div id="main">
                    <div class="title">
                      <Icon type="ios-analytics-outline" size="20" />最近一小时访问情况
                    </div>
                    <div
                      class="centent"
                      ref="main"
                      style="height:400px;background-color:#fff;position:relactive"
                    ></div>
                  </div>
                </Col>
                <Col :xs="24" :lg="6">
                  <div class="title">
                    <Icon type="ios-analytics-outline" size="20" color="#f56" />当前在线
                  </div>
                  <div class="centent">
                    <P>12:00:00</P>
                    <h2>56</h2>
                    <P>在线访问人数</P>
                    <i>一秒后更新</i>
                  </div>
                </Col>
                <Col :xs="24" :lg="6">
                  <div class="title">
                    <Icon type="ios-analytics-outline" size="20" color="#f56" />当前活跃度
                  </div>
                  <div
                    class="centent"
                    ref="active"
                    style="width:100%;height:160px;background-color:#fff;margin:0 auto"
                  ></div>
                </Col>
                <Col :xs="24" :lg="12" style="margin-top:10px">
                  <div id="main">
                    <div class="title">
                      <Icon type="ios-analytics-outline" size="20" color="#f56" />平均评价
                    </div>
                    <div class="footer">
                      <div>
                        <h2>{{valueHalf}}</h2>
                        <Rate allow-half v-model="valueHalf" />
                      </div>
                      <p>当前评价没有任何波动</p>
                      <Progress :percent="25" />
                      <Progress :percent="45" status="active" />
                      <Progress :percent="65" status="wrong" />
                      <Progress :percent="100" />
                    </div>
                  </div>
                </Col>
                <Col :xs="24" :lg="6">
                  <div id="main">
                    <div class="title">
                      <Icon type="ios-analytics-outline" size="20" color="#f56" />客户满意度
                    </div>
                    <div class="footer">
                      <div class="top">
                        <h2>865</h2>
                        <div>
                          <img src="../../assets/img/icon-happy.89cfbfe9.svg" alt />
                          <p>正面评价</p>
                        </div>
                        <h2 style="color:green">82%</h2>
                      </div>
                      <div class="top">
                        <h2>62</h2>
                        <img src="../../assets/img/icon-sad.22a51559.svg" alt />
                        <p>反面评价</p>
                        <h2 style="color:red">9%</h2>
                      </div>
                    </div>
                  </div>
                </Col>
                <Col :xs="24" :lg="6">
                  <div id="main">
                    <div class="title">
                      <Icon type="ios-analytics-outline" size="20" color="#f56" />本月目标
                    </div>
                    <div class="footer">
                      <Circle :percent="80">
                        <span class="demo-Circle-inner" style="font-size:24px">80%</span>
                      </Circle>
                    </div>
                  </div>
                </Col>
              </Row>
            </div>
          </div>
          <div class="footer">
            <div>
              <p>官网</p>
              <p>社区</p>
              <p>平台</p>
            </div>
            <div>
              <p>Copyright © 2019 北京视图更新科技有限公司</p>
            </div>
          </div>
        </Content>
      </Layout>
    </Layout>
  </div>
</template>
<script>
import echarts from "../../../node_modules/echarts";
export default {
  data() {
    return {
      loading: false,
      isCollapsed: false,
      value: "",
      value1: false,
      showTable: false,
      flagMonitor: true,
      valueHalf: 4.5,
      monitor: [
        {
          icon: "",
          title: "123K",
          text: "访问人数",
          img: [1, 2, 3],
        },
        {
          icon: "",
          title: "54k",
          text: "点击量",
          click: "115%",
        },
        {
          icon: "",
          title: "123K",
          text: "到达量",
          arrival: "15%",
        },
        {
          icon: "",
          title: "123K",
          text: "转化率",
          aransform: "65%",
        },
      ],
      columns7: [
        {
          title: "规则名称",
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
          title: "描述",
          key: "description",
        },
        {
          title: "服务调用次数",
          key: "service",
        },
        {
          title: "状态",
          key: "status",
        },
        {
          title: "上次调度时间",
          key: "time",
        },
        {
          title: "操作",
          key: "action",
          width: 250,
          align: "center",
          render: (h, params) => {
            return h("div", [
              h(
                "a",
                {
                  props: {
                    type: "primary",
                    size: "small",
                  },
                  style: {
                    marginRight: "5px",
                    textAlign: "right",
                    borderRight: "1px solid #ccc",
                    paddingRight: "5px",
                  },
                  on: {
                    click: () => {
                      this.show(params.index);
                    },
                  },
                },
                "编辑"
              ),

              h(
                "a",
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
                "订阅警报"
              ),
            ]);
          },
        },
      ],
      data6: [
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
        {
          name: "John Brown",
          description: 18,
          address: "New York No. 1 Lake Park",
          service: "650万",
          status: "运行中",
          time: "2020-06-11 07:25:20",
        },
      ],
      options: {
        tooltip: {
          trigger: "axis",
          axisPointer: {
            type: "cross",
            label: {
              backgroundColor: "#fff",
            },
          },
        },
        legend: {
          data: ["浏览量", "游客数"],
        },
        toolbox: {
          feature: {
            saveAsImage: {},
          },
        },
        grid: {
          left: "3%",
          right: "4%",
          bottom: "3%",
          containLabel: true,
          width: "100%",
        },
        xAxis: [
          {
            type: "category",
            boundaryGap: false,
            data: [
              "10:00",
              "10:15",
              "10:25",
              "10:40",
              "10:48",
              "10:56",
              "11:00",
            ],
          },
        ],
        yAxis: [
          {
            type: "value",
          },
        ],
        series: [
          {
            name: "浏览量",
            type: "line",
            stack: "总量",
            areaStyle: {},
            data: [120, 132, 101, 134, 90, 230, 210],
          },
          {
            name: "游客数",
            type: "line",
            stack: "总量",
            areaStyle: {},
            data: [220, 182, 191, 234, 290, 330, 310],
          },
        ],
      },
      options1: {
        angleAxis: {},
        radiusAxis: {
          type: "category",
          data: ["周一", "周二", "周三", "周四"],
          z: 10,
        },
        polar: {},
        series: [
          {
            type: "bar",
            data: [1, 2, 3, 4],
            coordinateSystem: "polar",
            name: "A",
            stack: "a",
          },
          {
            type: "bar",
            data: [2, 4, 6, 8],
            coordinateSystem: "polar",
            name: "B",
            stack: "a",
          },
          {
            type: "bar",
            data: [1, 2, 3, 4],
            coordinateSystem: "polar",
            name: "C",
            stack: "a",
          },
        ],
        legend: {
          show: true,
          data: ["A", "B", "C"],
        },
      },
    };
  },
  mounted() {
    let main = this.$refs.main;
    var myChart = echarts.init(main);
    myChart.setOption(this.options);
    let active = this.$refs.active;
    var myChart1 = echarts.init(active);
    myChart1.setOption(this.options1);
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
    showMonitor() {
      this.flagMonitor = true;
      this.showTable = false;
    },
    showFun() {
      this.showTable = true;
      this.flagMonitor = false;
    },
    loadingFun() {
      this.loading = !this.loading;
      setTimeout(() => {
        this.loading = !this.loading;
      }, 2000);
    },
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
