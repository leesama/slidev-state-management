# redux的弊端
<br>
Redux 的利弊已讨论太多，简单来说，开发者关心的是 "使用"，而 Redux 关心的是 "哲学"。

之前开玩笑说，其实 Redux 用一行代码就可以表示，却写出了论文规格昏昏欲睡的文档：
```js
createStore = (reducer, state) => ({ dispatch: (action) => (state = reducer(state, action)) });
```