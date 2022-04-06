
# 我们真的需要redux、mobx吗？

<!--
首先我们要明白，Redux 和Mobx都是一个特定时期的产物， 在React没有提供更好的状态管理方法之前，Redux 能够帮助使用React的开发者-把， Mobx也能提供一种全新的状态管理理念。
不过，React 是在持续发展的，光是Context API的改进，几乎就可以取代react-redux和mobx-react的作用。实际上，react-redux 和mobx-react两者的实现都依赖于React的Context功能。
以Redux为例，它相较于React Context还有哪些特点呢?
Redux有更清晰的数据流转过程，配合Redux Devtools的确方便Debug，代价就是我们必须要写哕嗦的action和reducer。
如果我们觉得应用并不需要Redux这样的增强功能，那完全就可以直接使用React的Context。
当然，React 的Context还是过于简单了一-点
-->
