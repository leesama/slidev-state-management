---
layout: two-cols
---

# React 中的状态

<br>
<br>
<br>
<br>
<br>

# State

::right::

<v-click>

状态如何传递？

</v-click>

<v-click>

| 场景   | 状态    |
| ------ | ------- |
| 父子   | props   |
| 跨组件 | Context |

</v-click>

<!--
2013 年 5 月 React 诞生。
但 2015 年之前，大概都是 jQuery 的天下。
2015 年 3 月 React 0.13.0 发布，带来了 class 组件写法。
在 React class 组件时代，状态就是 this.state，使用 this.setState 更新。
为避免一团乱麻，React 引入了 "组件" 和 "单向数据流" 的理念。
有了状态与组件，自然就有了状态在组件间的传递，一般称为 "通信"。
父子通信较简单，而深层级、远距离组件的通信，则依赖于 "状态提升" + props 层层传递。
于是，React 引入了 Context，一个用于解决组件 "跨级" 通信的官方方案。
但 Context 其实相当于 "状态提升"，并没有额外的性能优化，且写起来比较啰嗦。为优化性能，一般会添加多个 Context，写起来就更啰嗦。在项目没那么复杂时，还不如层层传递简单。
-->
