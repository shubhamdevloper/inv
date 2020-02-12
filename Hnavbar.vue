<template>
    <div class="navbar-container">
        <div class="logo-div">
            <img class="logo" @click="onHome" src="../assets/logoo.png">
        </div>
        <div>
            <ul>
                <li><router-link :to="{ name:'login' }">SignIn</router-link></li>
                <li><router-link :to="{ name:'registration' }">SignUp</router-link></li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {
    name: "navigation-bar",
    methods:{
        onHome(){
            this.$router.push('/');
        }
    }
}
</script>

<style lang="scss" scoped>
.navbar-container{
    height:90px;
    width:100%;
    position:sticky;
    top:0px;
    background-image: url("../assets/nav1.jpg");
    //background-color:#6e6e6e;
    border:1px solid #355568;
    box-shadow: 2px 2px 20px #355568;

}
.logo-div{
    margin-left:25px;
    float:left;
    margin-top: 7px;
}
.logo{
    height: 70px;
    width:auto;
    cursor: pointer;
}
ul{
    display: flex;
    justify-content: flex-end;
    list-style-type: none;
    margin-top: 35px;
}
ul li{
    margin-right:50px;
    float:left;
    cursor: pointer;
    font-size:22px;
}
ul li a{
    text-decoration: none;
    font-size:16px;
    font-weight: 600;
    color:white;
}
ul li a:hover{
    text-decoration: none;
    color:#990a39;
}
</style>