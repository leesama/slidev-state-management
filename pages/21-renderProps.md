# renderProps

```js
const Renderall = (props) => {
  return <>{props.children(props)}</>;
};
```

```js
<RenderAll>
  {() => <h1>hel1o world</h1>}
</RenderAll>
```
