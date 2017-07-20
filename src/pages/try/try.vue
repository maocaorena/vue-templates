<template>
	<div class="login">
		<div class="login-box">
			<el-card class="box-card" :header="title">
			  <el-input placeholder="请输用户名" v-model="userName">
			    <template slot="prepend">用户名</template>
			  </el-input>
			  <el-input placeholder="请输密码1111" v-model="password">
			    <template slot="prepend">密&nbsp;&nbsp;&nbsp;&nbsp;码</template>
			  </el-input>

			  <el-button type="primary" style="width:100%;" @click="submit">登录啊</el-button>
			</el-card>
			<button id="btn">
				111
			</button>
			
	   </div>
	</div>
</template>
<script>
export default {
  name: 'login',
  data(){
  	return {
  		title:"登录",
  		userName:"",
  		password:""
  	}
  },
  methods:{
  	submit(){
  		alert("1")
  	}
  },
  mounted(){
  	var ss = document.getElementById('btn');
  	btn.addEventListener("click",function(){
  		mmm()
  	},false);
  	function mmm(){
  		alert('11')
  	}
  }
}	
</script>

<style lang="less" scoped>
.login{
	.login-box{
		margin: 100px auto;
		width: 400px;
		.el-input{
			margin: 20px 0;
		}
		.box-card{
			text-align: center;
			color: #20A0FF;
		}
	}

}
</style>