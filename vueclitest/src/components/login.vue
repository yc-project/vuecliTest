<template>
   <div id="loginApp" class="loginApp">
    <div style="width:100%;height:60px;background-color:#800000;">
      <div style="height:10px"></div>
      <font style="margin-left:700px;font-weight:bolder;font-size:25px;color:white">登录</font>
    </div>
   

    
  </div>
</template>

<script>
export default {
  name: 'login',
  data:function(){
    return{ 
      username: "",
      userpwd: ""
      }
  },
  methods:{

    login() {
          if (this.username == "yc" && this.userpwd == "123") {
            window.alert("登录成功！是否确认跳转？")
           // window.location.href="MenuFirst.html"
          } else {
            window.alert("登录失败")
           
          }
        },
         register(){
           console.log("注册")
          //window.location.href="Regist.html"
         }
  },
  props: {
    msg: String
  }
}
</script>


<style scoped>
 .loginApp{
  
   width:100%;
   height: 100%;
 }

</style>
