
### 说明
> 这是安全教育平台一键完成作业的一个例子，这个例子是针对《2019年全国中小学生防灾减灾安全教育》这课做的，如果要写其它作业的一键完成可以按照这样的套路

### 思路
> 先用okhttp进行post键值模拟登录，然后获取到用户的cookie再将获取到的cookie设置到webview中（目的是快速对两个不同的模块进行快速登录），然后对webview进行动态注入js代码并执行（用于对作业的单选题和提交按钮的模拟点击），主要思路就是这样

### 使用
--- json
获取本地json内容 一定要设置 格式如下然后以此类推
		 [{
		 	"admin" : "第一个账号",
		 	"password" : "第一个密码"
		 } , {
		 	"admin" : "第二个账号",
		 	"password" : "第二个密码"
		 }]
---
