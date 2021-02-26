### script 的 async 跟 defer 的区别？

> 考点
> 
> 浏览器渲染原理

浏览器在执行html的时候，如果遇到`<script>`时就会停止去渲染页面去下载和执行js文件，而指定`defer`和`async`的时候就能控制js的下载和执行

- defer:告诉浏览器立即下载，但延迟执行，消除阻塞；但是这个延迟执行会在`DOMContentLoaded`事件执行之前来运行
- aysnc:并行请求脚本，消除阻塞，但是脚本执行但先后顺序无法保证
