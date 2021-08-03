# Vue+Axios ColdIce Player

#### 介绍
基于Vue.2x + Axios开发的网页音乐播放器  调用接口属于网易云音乐 NodeJS 版 API

#### 软件架构
Vue.2x 渐进式框架
Axios 基于 Promise 的 HTTP 客户端，可以工作于浏览器中，也可以在 node.js 中使用




#### 使用说明

1.  歌曲搜索：P1 服务器返回数据比较复杂时，获取时候注意层级结构 P2 通过审查元素快速定位需要操纵的元素
2.  歌曲播放：P1 点击播放(v-on 自定义参数简化编码) P2 歌曲地址获取(接口 地址id) P3 歌曲地址设置 (src改变 v-bind)
3.  歌曲封面：P1 点击播放(增加逻辑) P2 歌曲封面获取(接口 地址id) P3 歌曲地址设置(src改变 v-bind操纵属性)
4.  歌曲评论：P1 点击播放 P2 歌曲评论获取 P3 歌曲评论渲染 (通过v-for生成列表)
5.  播放动画：P1 监听音乐播放(v-on play)  audio的play事件在音乐播放的时候触发 P2 监听音乐暂停(v-on pause) audio的pause事件在音乐播放的时候触发 P3 操纵类名(v-bind 对象)
6.  MV播放：P1 MV图标显示(v-if) P2 MV地址获取(接口) P3 遮罩层(v-show v-on) P4 MV地址设置(v-bind)