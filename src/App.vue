<template>
    <div class="container">
        <div class="nav">
          <a class="logo" href="/">企业帮-企业经营之道</a>
          <img class="logo1" src="./assets/navlogo.png">
        </div>
        <div class="hu">
            <div class="tab2">
                <img class="picture" src="./assets/tttttt.jpg">
            </div>
            <div class="tab3">
                <a class="logintop" href="/" @click="login12()">
                    <div class="loginfrist">
                        <img class="loginfrist1" src="./assets/1212.jpg">
                    </div>
                    <div class="loginsecond">
                        <p class="logocode">苏州骏汽车</p>
                    </div>
                    <i class="fa fa-pencil"></i>
                </a>
                <div class="loginbutton">
                    <div style="width:200px; margin-top:10px">
                       <!--<input type="button" value="弹出窗口" id="btntc" style="width:100px; height:30px; font-size:18px;" />-->
                    </div>
                    <input class="name" placeholder="账号" v-model="userName">
                    <input class="password" placeholder="密码" v-model="password" type="password">
                    <div class="rempass" >
                        <div class="xuanze">
                            <input type="checkbox" name="vehicle" value="Bike">
                            <tenant-change></tenant-change>
                        </div>
                        <div class="jizhu">
                            <p class="testone">记住密码</p>
                        </div>
                    </div>
                    <button type="button" @click="login()" class="but">登录</button>
                    <p class="ttt">@2020苏州新序软件 Ver.1.2.5 [20200916]</p>
                    <p class="yyy">苏ICP备15019353号</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    // import HelloWorld from './components/HelloWorld.vue'
    //import $ from 'jquery'
    export default {
        name: 'App',
            el: '#app',
        data:function () {
            return{
                userName:'',
                password:'',
            }
        },
        methods: {
            login() {
                var b = true;
                if (this.userName == "") {
                    b = false;
                    alert('请输入用户名！')
                }
                else{
                    if (this.password == "") {
                        b = false;
                        alert('请输入密码！')
                    }
                }
                if (b) {
                    if(this.userName=="admin")
                    {
                        if(this.password=="123456")
                        {
                            window.location.href="https://www.baidu.com/";
                        }
                        else {
                            alert('密码错误！')
                        }
                    }
                    else{
                        alert('账号错误！')
                    }
                }
            },
            login12(){
                alert('nihao')
            },
        }
        // $(document).ready(function() {
        //
        // })
            // data: {
            //     // message: 'Runoob',
            // }
        // created() {
        //     this.loadXMLDoc();
        // },
        // methods: {
        //     loadXMLDoc()
        //     {
        //         //post:http://localhost:6298/api/TokenAuth/Demopost
        //         //参数：tenantId，类型：int
        //         $.ajax({
        //             type: "get",
        //             // url: "http://localhost:6298/api/TokenAuth/Demo",
        //             url: "http://localhost:6298/api/TokenAuth/Demo",
        //             dataType:"json", //预期服务器返回数据的类型
        //             data:{
        //                 tenantId:'4',
        //             },
        //             success:function(data){
        //                 console.log(data)
        //             },
        //             error:function(jqXHR){
        //                 alert("发生错误："+ jqXHR.status);
        //             }
        //         });
        //
        //     }
        // }
    }
</script>
<style>
    @import"./assets/a.css";
</style>
