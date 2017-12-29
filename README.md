# bootstrap-practice

## 简介

夯实Bootstrap基础，欧耶！

## 心法

### V3篇

#### Examples: 01-Starter Template 

- 此例所用组件
  - Navbar

Navbar使用方法

  - Navbar的基本结构
    - 第一层包个div.navbar
    - 第二层再包个div容器div.container
    - 第三层有讲究的
    - 第3.1层为div.navbar-header，注意header里只能包含"商标+汉堡"，即.navbar-brand和.navbar-toggle
    - 第3.2层为折叠显示层，最好又拿个div包起来，加个.collapse.navbar-collapse，因为我们要时刻牢记Bootstrap的核心原理：单一职责原则(SRP)
    - 在3.2层下，又可以包含ul、form等各类元素，但Bootstrap都为我们设计好了navbar对于类，如form对应.navbar-form、ul对应.nav.navbar-nav等，单一链接对应.navbar-link等等
  - Navbar中JS组件使用
    - 在触发元素上添加自定义属性`data-toggle="collapse"`
    - 如果触发元素是a的话就在属性添加指向的id`href="#menu"`
    - 如果触发元素是其他就添加自定属性`data-target="myMeny"`

#### Examples: 03-Jumbotron

- 此例所用组件
  - Navbar
  - Grid
  - Jumbotron

Jumbotron
  - Jumbotron直译为超大屏幕
  - 样式挺简单的
  - 上下内边距30px，下margin30px，背景#eee
  - 嗯，就是把内容好好放中间显示，下面的衔接内容也留出很大空白，突显啊！
  - 你看，Jumbotron里的p也把字体放大了，

Grid
  - 此例中Grid就太简单了
  
 其它
   - 原来`.btn-default`背景色是白色啊
   - Bootstrap里可以多用几个`.container`把内容定宽居中，把不相关的内容独立出来，footer就是最后面睡着
   - p元素里可以放`.btn`

#### Examples: 04-Narrow Jumbotron

狭小的超宽屏
感觉这个例子中整啥新的，就有个修改定宽容器。

  - 在媒体查询里，如果屏幕宽度大于768px，就修改定宽容器.container的宽度为730px

#### Examples: 05-Justified-Nav

这个小导航坑了我一哈，我要把你吃掉。

Nav导航组件

- Bootstrap中的导航组件都依赖同一个 `.nav` 类，状态类也是共用的。改变修饰类可以改变样式。
- .nav 得加载ul上
- `.nav` 进来就先把ul的padding-left左内边距和下外边距清零，再去除li的小点点
- 然后给子元素li加相对行为和设块级元素，再给li的子元素a：设为相对定位和块级元素，内边距撑开父元素；
- 真到是基础类
- `.nav`整出来的li因为是块级元素，要占一行
- `.nav-justified` 为什么li规规矩矩排列一行，因为`display: table-cell;`

#### Examples: 06-Cover

全屏填充背景色的网页一个。

步骤

  - body元素高度100%和背景色，字体颜色
  - .site-wrapper：全局100%撑满父元素，显示为表格模式，高度也撑开，黑body盒子套一个内阴影

----------

### V4篇