# renderProps的优势

```js
const withLogin = (Component) => {
  const NewComponent = (props) => {
    const userName = getUserName();
    if (userName) {
      return <Component {...props} userName={userName} />;
    } else {
      return null;
    }
  };
  return NewComponent;
};

```

用hoc实现的该组件要求组件必须由于userName才能正常显示

```js
<Login>
  {(props) => {
    const { userName } = props;
    return <TheComponent {...props} name={userName} />;
  }}
</Login>;
```