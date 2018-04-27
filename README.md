# browserCookie
用 jQuery 封装 Cookie 的设置、获取、删除方法

## 插件用法
```html
<script src="jquery.min.js"></script>
<script src="browserCookie.min.js"></script>
```
引入上面两个文件之后，即可调用该插件了：
```javascript
<script type="text/javascript">
//设置 Cookie
$.setCookie(name,value,expiredays,path,domain,secure);
//获取 Cookie
$.getCookie(name);
//删除 Cookie
$.deleteCookie(name);
</script>
```

## 参数说明
**setCookie(name,value,expiredays,path,domain,secure)**
- name：Cookie 名；
- value：Cookie 值；
- expiredays：Cookie 在 expiredays 天后会过期；
- domain：可以访问该 Cookie 的域名；
- path：可以访问该 Cookie 的路径；
- secure：设置该 Cookie 是否只能通过 https 来传递；
- domain 和 path 这两个选项共同决定了 cookie 能被哪些页面共享；

## 示例
- 初次访问填写 name，再次访问弹出欢迎信息：
  [demo1](https://alvinyw.github.io/Blog/browserCookie/demo1.html)
  
- 初次访问填写 name 和 password，再次访问自动补全相应表单：
  [demo2](https://alvinyw.github.io/Blog/browserCookie/demo2.html)
  
- 提示最近一次访问网站的时间：
  [demo3](https://alvinyw.github.io/Blog/browserCookie/demo3.html)
  
- 当第一次访问网站是弹出提示信息：
  [demo4](https://alvinyw.github.io/Blog/browserCookie/demo4.html)