# Cat React CMS

开箱即用的中台前端/设计解决方案。
​


## 待支持特性


- [ ]  **TypeScript**: 应用程序级 JavaScript 的语言
- [ ]  **区块**: 通过区块模板快速构建页面
- [ ]  **常见设计模式**：提炼自中后台应用的典型页面和场景
- [ ]  **最新技术栈**：使用 React/antd 等前端前沿技术开发
- [ ]  **响应式**：针对不同屏幕大小设计
- [ ]  **Mock 数据**：实用的本地数据调试方案
- [ ]  **配置化**：路由，操作，展示页面配置化，实现低code平台
- [ ]  **微前端**：接入微前端方案，实现项目间的高效复用
- [ ]  **主题**：可配置的主题满足多样化的品牌诉求
- [ ]  **国际化**：内建业界通用的国际化方案
- [ ]  **UI 测试**：自动化测试保障前端产品质量



## 模板


```
- Dashboard
  - 分析页 （实践一下antv：https://antv.vision/）
  - 监控页
  - 工作台
- 表单页（二次封装）
  - 基础表单页 
  - 分步表单页
  - 高级表单页
- 列表页（二次封装）
  - 查询表格（结合搜索+表单+路由）
- 详情页
  - 信息展示页（二次封装）
  - 微前端实践页（通过微前端嵌入其他项目）
- 用户（排期可以往后放）
  - 用户中心页
  - 用户设置页
- 异常
  - 403 无权限
  - 404 找不到
  - 500 服务器出错
- 帐户
  - 登录
  - 注册
  - 注册成功
- 配置
  - 路由配置（渲染侧边栏）
  - 页面配置（控制模块，操作是否显示）
  - 操作配置（渲染公共操作）
```


## 使用


```bash
框架搭建后发到npm上再写
```


更多信息请参考 使用文档。


## 支持环境（还不确定）

有一些功能之后检测一下

```
function getBrowserInfo(){
	var agent = navigator.userAgent.toLowerCase() ;
	
	var regStr_ie = /msie [\d.]+;/gi ;
	var regStr_ff = /firefox\/[\d.]+/gi;
	var regStr_chrome = /chrome\/[\d.]+/gi ;
	var regStr_saf = /safari\/[\d.]+/gi ;
	//IE
	if(agent.indexOf("msie") > 0){
		return agent.match(regStr_ie) ;
	}

	//firefox
	if(agent.indexOf("firefox") > 0){
		return agent.match(regStr_ff) ;
	}
	
	//Chrome
	if(agent.indexOf("chrome") > 0){
		return agent.match(regStr_chrome) ;
	}
	
	//Safari
	if(agent.indexOf("safari") > 0 && agent.indexOf("chrome") < 0){
		return agent.match(regStr_saf) ;
	}
}
//	（2）然后获取版本号
		var browser = getBrowserInfo() ;
		alert(browser); 
		var verinfo = (browser+"").replace(/[^0-9.]/ig,""); 
		alert("verinfo=="+verinfo);
————————————————
版权声明：本文为CSDN博主「weixin_43812512」的原创文章，遵循CC 4.0 BY-SA版权协议，转载请附上原文出处链接及本声明。
原文链接：https://blog.csdn.net/weixin_43812512/article/details/84562170
如何判断当前浏览器是不是当前项目能够兼容的浏览器
```


## 参与贡献


我们非常欢迎你的贡献，你可以通过以下方式和我们一起共建 ：


- 在你的公司或个人项目中使用Cat React CMS。
- 通过 Issue 报告 bug 或进行咨询。
- 提交 Pull Request 改进 CRC 的代码。