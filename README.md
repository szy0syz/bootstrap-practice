# bootstrap-practice

## 简介

夯实Bootstrap基础，欧耶！

## 心法

### V3篇

#### Examples: Starter Template 

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

### V4篇