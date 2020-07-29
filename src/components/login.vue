<style>
    .container{
        display: flex;
        justify-content: center;
        position:relative;
        box-sizing:border-box;
        background: url("../assets/img/body.8aa7c4a6.svg");
        background-size: contain;
        width: 100%;
    }
    .form{
        width:100%;
        max-width: 380px;
        overflow: hidden;
    }
    form{
        width: 100%;
        margin-top:45px;
    }
    .ivu-input-group .ivu-input{
        height: 100%;
    }
    .ivu-input-group{
        height: 40px;
    }
    form div{
        width: 100%;
    }
    .logo img{
        width: 100%;
    }
    .title{
        color: #666;
        margin:10px 0;
    }
    .ivu-checkbox-wrapper{
        float: left;
    }
    #check a{
        float: right;
    }
    .ivu-btn-primary{
        width: 100%;
    }
    .other .ivu-row{
        width: 100%;
    }
    .ivu-col-span-12{
        display:flex;
    }
    .other img{
        width: 25px;
        height: 25px;
        margin-left:10px
    }
   
</style>
<template>
  <div>
      <myHeader></myHeader>
     <div class="container">
    <div class="form">
      <Form ref="formInline" :model="formInline" :rules="ruleInline" inline >
          <FormItem prop="user">
              <Input type="text" v-model="formInline.user" placeholder="Username">
              <Icon type="ios-person-outline" slot="prepend"></Icon>
              </Input>
          </FormItem>
          <br/>
          <FormItem prop="password">
              <Input type="password" v-model="formInline.password" placeholder="Password">
              <Icon type="ios-lock-outline" slot="prepend"></Icon>
              </Input>
          </FormItem>
          <br/>
          <FormItem id="check">
              <Checkbox v-model="single">自动登录</Checkbox><a href="#">忘记密码</a></Checkbox>
          </FormItem>
          <br/>
          <FormItem>
              <Button type="primary" @click="handleSubmit('formInline')">登录</Button>
          </FormItem>
      </Form>
      <div class="other">
        <Row>
            <Col span="6"><p>其他登录方式</p></Col>
            <Col span="12">
                <img src="../assets/img/icon-social-qq.2cf4276d.svg" alt="">
                <img src="../assets/img/icon-social-wechat.c69ec08c.svg" alt="">
                <img src="../assets/img/icon-social-weibo.cbf658a0.svg" alt="">
            </Col>
            <Col span="6"><a href="#">注册账户</a></Col>
        </Row>
      </div>
     
    </div>
  </div>
  </div>
 
</template>
<script>

import myHeader from "./myHeader";
export default {
  data() {
    return {
    single:'false',
      formInline: {
        user: "admin",
        password: "123456",
      },
      ruleInline: {
        user: [{ required: true, message: "账号不能为空", trigger: "blur" }],
        password: [
          { required: true, message: "密码不能为空", trigger: "blur" },
          {
            type: "string",
            min: 6,
            message: "密码长度6-16个字符",
            trigger: "blur",
          },
        ],
      },
    };
  },
  components: {
    myHeader,
  },
  methods: {
    handleSubmit(name) {
      this.$refs[name].validate((valid) => {
        if (valid) {
          this.$Message.success("登录成功");
          this.$router.push('/menu')
        } else {
          this.$Message.error("密码或用户名错误");
        }
      });
    },
  },
};
</script>
