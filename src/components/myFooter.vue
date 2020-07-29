<style>
    .footer{
        position: absolute;
        bottom: 50px;
        left: 0;
        right: 0;
        margin: 0 auto;
    }
    .footer div:first-child{
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .footer p{
        margin-left: 10px;
        color: #666;
    }
</style>
<template>
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
</template>

<script>
export default {
  name: "myFooter",
};
</script>

<style>
</style>
