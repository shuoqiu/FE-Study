ELWG前端学习小组任务（副本）
=====

## 任务说明

* 带`+`号的为副本难度，1-5个`+`号分别对应1-5星难度

## 团队副本任务

### ELWG Contacts（通讯录）

#### 需求分析

1. 单页应用，没有任何页面跳转
2. 通讯录以表格形式呈现，每一条记录包括姓名，年级，邮箱，电话，生日，导师，照片等信息
    * 由于照片尺寸不一，为避免破坏表格结构，照片在表格中以一个小图标表示，点击图标再弹出照片
3. 整个通讯录提供一个添加按钮，点击后弹出“添加通讯录”对话框
    * 年级用下拉框，选项如“2013级学硕”“2014级工硕”
    * 导师用下拉框
    * 照片让用户自行上传
4. 每一条记录可以编辑或删除
    * 点击编辑，弹出“添加通讯录”对话框，预填内容
    * 点击删除，弹出警告框，确认才可以删除
5. 提供一个类似淘宝商品多级分类筛选的功能，点击每一项都可以进行一次内容筛选。以下是参考分类：
    * 年级：2013级学硕 2013级工硕 2014级学硕 2014级工硕
    * 导师：许炜 程文青 夏天
6. 一开始进入页面时，显示所有的通讯录（也就是没有任何筛选条件），但要按照每页10个条目分页显示

【进阶需求】

1. 用户上传照片时，提供剪裁功能，保存剪裁后的图片
2. 年级和导师选项不要“写死”在代码中，而是可通过一个“通讯录管理页面”进行配置
3. 上传照片环节，改为直传七牛云存储（需要学习七牛API和SDK）
3. 表格中显示照片，为保证表格结构一致，照片以相同的尺寸进行缩放显示

#### 要求

* 公共要求
    * 学习[CodeIgniter 3.x](http://codeigniter.org.cn/user_guide/)框架
    * 学习REST API，并根据需求分析设计一套API，~~以书面形式提交给技术导师~~直接在[RAP](http://rap.taobao.org/)（可视化API编辑网站）上编辑好了给技术导师查看。参考资料：[REST API Tutorial](http://www.restapitutorial.com/)、[阮一峰RESTful API设计指南](http://www.ruanyifeng.com/blog/2014/05/restful_api.html)
* 前端要求
    * 根据需求分析，设计该单页应用的**线框图**。推荐使用[ProcessOn](https://www.processon.com/i/56653f6be4b0fd92998feae3)或者Axure画
    * 调研**至少3款**CSS框架，简要对比分析它们的优劣，并给出你选择其中一款的理由。需要写一份简短的调研报告提交给技术导师。
    * 【**学习完CI框架，提交API设计、线框图、CSS框架调研报告**后，再开放下面具体的技术要求】
* 后端要求
    * 根据需求分析，设计Mysql的表结构。
    * 【**学习完CI框架，提交API设计、线框图、Mysql表结构**后，再开放下面具体的技术要求】

## 单人副本任务

### 可视化的Web API设计网站【Web网站方向 ++】

* 目标：
    1. 实现一个可视化的API设计网站，填补国内空白
    2. 通过本项目进一步熟练使用Web网站开发的工作流
    3. 培养最基本的Web网站审美能力
* 要求：
    1. 自己从零开始搭建项目
    2. 使用技术：自选一门后端语言（PHP/Python/Node.js等等）、框架及模板引擎；LESS/Sass+自选一款CSS框架；Javascript模块化；Grunt部署站点
    3. 界面美观，扁平化风格，布局、视觉、交互均自行设计（注意移动端布局的设计）
    4. 支持响应式设计，布局可以在PC端、iPad及主流大屏手机正常显示

### 全局播放器【Web组件方向 +++】

* 目标：
    1. 实现一个全局播放器，满足青桔网的进阶需求
    2. 提高发掘前端组件的能力，提高阅读源码及编写组件的能力
* 要求：
    1. 自行查找音频播放相关的资料，从零实现青桔网播放器的一个子集
    2. 设计一种模式，实现播放器的全局播放功能（页面跳转不中断播放），参见[QQ音乐](http://y.qq.com/)
    3. 必须以成本最低的方式兼容青桔网现有的架构与代码

### 贪吃蛇网络对战【游戏方向 ++++】

* 目标：
    1. 实现一个贪吃蛇的网络对战游戏
    2. 理解单机游戏和简单网络游戏的基本开发方式
* 要求：
    1. 底层实现不做限制，基于div、基于HTML5 canvas、基于游戏引擎均可
    2. 良好的服务器端接口设计，只要客户端遵循API规范，就可以接入对战
    3. 界面美观，自行设计
