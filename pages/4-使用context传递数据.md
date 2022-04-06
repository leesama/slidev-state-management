
# context的问题
Context 其实相当于 "状态提升"，并没有额外的性能优化，且写起来比较啰嗦。
为优化性能，一般会添加多个 Context，写起来就更啰嗦。在项目没那么复杂时，还不如层层传递简单。
```js
const MyContext = React.createContext(defaultValue);
function App() {
  return (
    <Context1.Provider>
      <Context2.Provider>
        <Context3.Provider>
          <div className="App">
            <Header />
            <Main />
            <Footer />
          </div>
        </Context3.Provider>
      </Context2.Provider>
    </Context1.Provider>
  );
}
```

<!--
如果把所有数据写在同一个context中 任何数据改变都会导致依赖context的组件重新渲染、
例如 context中存有{a,b,c}

如果只想获取a属性， b、c属性的改变也会导致只想获取a属性所在的组件重新渲染 

因为他们在同一个对象里面
-->
