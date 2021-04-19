---
title: graduation-project
date: 2021-04-18 19:42:53
tags: 
- Vue.js
- Element Plus
- Python
- Flask
- MySQL
categories: Software Engineering
---
# 网站名（暂定小说阅读网站）
## 一. 项目创建
使用Vue3
1. ```vue create reading-vue```
2. 对项目做预设（pick a preset）
   1. Manually select features
   2. Choose Vue version + Babel +  Linter / Formatter
   3. 3.x
   4. Use history mode for router? y
   5. ESLint + Standard config
   6. Lint on save
   7. In dedicated config files
3. 将项目托管到GitHub上
   1. E:\graduation-project目录下```git clone https://github.com/gitEast/read-novel.git```
   2. 除.git文件夹外都复制进read-novel文件夹下
   3. 在read-novel文件夹下，cmd：```git add .```
   4. cmd：```git commoit -m "初始化“```
   5. cmd：```git push```
4. 划分项目目录


## 二、标准规定
1. 页面主要宽度：1100px
2. border-radius: 15px

## 2021.03.09
### nav-bar完成
1. NavBar.vue：将nav-bar左右分割，左边是logo，右边是Library | Discuss | Login
2. NavBarRight.vue：由于右侧三个是链接，暂且用slot替代
   1. 设置文字居中，line-height
   2. 用div实现竖杠，宽1px，高1.5rem（字体大小），使用子绝父相使得竖杠垂直居中
3. FinishedNavBar.vue：放就是了
4. **存在问题**：logo未完成，右侧三个是链接未完成


### home的搜索框(search-bar)
1. 分三个部分，search-select + search-input + search-btn
2. SearchBar.vue：
   1. 使用Element ui的select选择器，制作search-condition

## 2021.03.10
### search-bar完成
1. 分三个部分，search-select + search-input + search-btn
2. SearchBar.vue：没有使用element-ui
3. search-btn中使用了子绝父相
4. **也需要改的问题**：button的定位问题


### home的轮播图
1. 放上的DOM元素，CSS未调整

## 2021.03.11
### home的轮播图
1. 决定从图片改成一句名人名言，背景色灰色

## 2021.03.15
### home的轮播图 完成
1. 分成四个部分：句子 + 左边按钮 + 右边按钮 + 实心圆列表
2. 句子
   1. 使用currentIndex控制当前句子显示
   2. CSS没什么问题
   3. 轮播效果：开启定时器→轮播
3. 左边按钮：
   1. 按钮被hover和active都有颜色变化，深入色
   2. 点击后：清除定时器→currentIndex变化→重启定时器
   3. **开启定时器是个方法啊！！！要()的！！！**
4. 右边按钮
5. 实心圆：道理同按钮差不多
   1. 因为选择器权重而出现的css无法实现的现象，使用```!important```解决

## 2021.03.26
### 最终完成的首页的两个小说卡片
1. 分成两个部分，但 是一样的结构：BookCard
2. BookCard分成两部分：标题 + book-card-item
3. book-card-item又分成两部分：小说标题 + 作者名
4. **重点**：组件套组件，如果内部组件是不确定个数的，则外部组件只需要一个```slot```，内部组件使用时通过```v-for```完成

## 2021.03.27
### 底部
1. 分成三部分：链接 + 邮箱图片 + copyright
2. 链接：使用flex布局使它们居中
3. 邮箱图片：
   1. 由于hover的切换有点麻烦，将邮箱图片作为背景图片使用
   2. ```background-size: contain```将图片缩放至元素宽高的正好
   3. 使用相对定位，使背景图片居中
4. copyright：
   1. copyright图标：```&copy;```
   2. 空格：```&nbsp;```
   3. 中心的圆点：```&middot;```

## 20201.04.04
### 对Library实现路由跳转
1. 安装vue-router
   1. **注意**：vue-router与vue的版本号要配合好（差点没被搞死...）
   2. 由于vue的版本为3，vue-router的版本为4
2. 在src/router目录下，新建index.js文件
   1. 函数式引入vue-router
   2. 创建路由对象（使用路由懒加载）
   3. 导出路由
   4. 顺便：后置钩子改变网页title
3. 在main.js中使用路由对象
4. 在FinishedNavBar.vue中，对目标div加入点击事件，实现路由跳转

### Library页面
#### 选择标签部分 tags
1. 使用element-ui（原因：iview不支持vue-cli4，但element-ui支持）
2. 父组件接收子组件中tags的选中情况

#### 分页器 + table
1. 分页器和table的结合使用
   1. 没用过，所以感觉有点难，其实很简单
   2. 改变el-table的data就好了

### Discuss页面
1. 帖子item的封装
2. 分页器
3. 分页器与帖子结合
4. 总结：跟Library差不多，甚至更简单些

### 购买服务器
1. 服务器镜像：CentOS  7.4 64位，自带tomcat和MySQL
2. html页面放置地址：```/usr/local/src/apache-tomcat-9.0.1/webapps/ROOT/```

## 代码实现
https://github.com/gitEast/read-novel







## 补充
### Element UI使用（按需引入）
1. 安装element-plus：```npm install element-plus --save```
2. 借助babel-plugin-import，只引入需要的组件，减少项目体积：```npm install babel-plugin-import -D```
3. 修改babel.config.js
```javascript
module.exports = {
  plugins: [
    [
      "import",
      {
        libraryName: 'element-plus',
        customStyleName: (name) => {
          return `element-plus/lib/theme-chalk/${name}.css`;
        },
      },
    ],
  ],
};
```
4. 在main.js中引入需要的组件
```javascript
import { createApp } from 'vue'
import { ElButton, ElSelect } from 'element-plus';
import App from './App.vue';

const app = createApp(App)
app.component(ElButton.name, ElButton);
app.component(ElSelect.name, ElSelect);

/* or
 * app.use(ElButton)
 * app.use(ElSelect)
 */

app.mount('#app')
```
**注意**：使用ElSelect时，ElOption也要引入