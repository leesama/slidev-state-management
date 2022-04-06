# renderProps的应用

```js
const Auth = (props) => {
  const userName = getUserName();
  if (userName) {
    const allProps = { userName, ...props };
    return <React.Fragment>{props.login(allProps)}</React.Fragment>;
  } else {
    <React.Fragment>{props.nologin(props)}</React.Fragment>;
  }
};
<Auth
  login={({ userName }) => <h1>Hello {userName}</h1>}
  nologin={() => <h1>Please login</h1>}
/>;

```