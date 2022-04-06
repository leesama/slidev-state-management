# renderProps的应用

```js
const Login = (props) => {
  const userName = getUserName();
  if (userName) {
    const allProps = { userName, ...props };
    return <>{props.children(allProps)}</>;
  } else {
    return null;
  }
};
<Login>
{({userName}) => <h1>Hello {userName}</h1>}
</Login>
```