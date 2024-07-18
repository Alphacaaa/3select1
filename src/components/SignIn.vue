<script>
export default{
    data(){
        return{
            user:{
                email:'',
                password:''
            }
        }
    }
}
</script>

<template>
    <div class="container">
        <form>
            <h1>LOGIN</h1>
            <div class="form">
                <label>Email</label>
                <input type="email"v-model="user.email"/>
                <!-- <h1>{{ user.email }}</h1> -->
                
                
            </div>
            <div class="form">
                <label for="">Password</label>
                <input type="password" v-model="user.password">
                
                <!-- <h1>{{ user.password }}</h1> -->
            </div>
            <div class="forgotContainer">
                <RouterLink to="/register">register</RouterLink>
                <RouterLink to="/forgot">Forgot?</RouterLink>
            </div>
            
            <button type="submit">Submit</button>
            
        </form>
    </div>
    
</template>

<style scoped lang="scss">
    *{
        box-sizing: border-box;
        margin: 0;
        padding: 0;
        border: 1px solid black;
    }
    .container{
        width: 700px;
        height: 800PX;
        margin: auto;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    form{
        margin: auto;
        // display: flex;
        width: 500px;
        height: 600px;
        // justify-content: center;
        // align-items: center;
        // flex-wrap: wrap;
        h1{
            width: 31%;
            margin: auto;
            text-align: center;
        }
        .form{
            width: 100%;
            height: 20%;
            margin: auto;
            // display: flex;
            // justify-content: center;
            // align-items: center;
            // flex-wrap: wrap;
            // text-align: center;
            label{
                // width: 90%;
                font-size: 30px;
                // height: 50%;
                
            }
            input{
                width: 90%;
                height: 20%;
            }
        }
        .forgotContainer{
            display: flex;
            justify-content: space-between;
            width: 70%;
            margin: auto;
        }
        button{
            display: block;
            margin: 30px auto;
            width: 30%;
            height: 10%;
            font-size: 36px;
        }
    }
    
</style>