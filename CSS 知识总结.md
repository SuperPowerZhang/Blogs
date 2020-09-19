
# CSS动画相关知识总结
## 浏览器渲染原理
### 渲染原理
浏览器根据HTML渲染一棵HTML树，根据CDD渲染一棵CSS树
再把两棵树合并成一棵Render树
Layout布局（文档流，大小，位置等）
Paint绘制（边框，颜色，背景）等
Compose合成（根据层叠关系展示）
### 更新原理
Javascript对页面进行更新，最长需经过：Style>Layout>Paint>Composite
如想要提高更新页面渲染的性能：（1）优化js，省去Layout/Paint等步骤；（2）优化每一步中的操作

## CSS 动画的两种做法（transition 和 animation）
### transition
有translate、scale、rotate、skew四种形式的动画
配合transition过渡实现动画
### animation
用@keyframs进行关键帧的设置，在元素的animation属性上进行动画的时长、过渡方式、延迟、方向等设置

## 其他
### CSS动画是一项艺术
transition实现心跳动画：http://js.jirengu.com/humof/17/edit?html,css,js,output
annimation实现心跳动画：http://js.jirengu.com/humof/16/edit?html,css,output
