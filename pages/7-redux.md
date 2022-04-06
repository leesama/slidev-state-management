---
layout: two-cols
---

# redux
<br>

actionType.js
```js
const CHANGENAME= 'CHANGENAME'
```
actions.js
```js
const changeNameCreater = 
(name) => ({type:CHANGENAME,data:name})
```
reducer.js
```js
const initialState = { name:'tutu'}
function modifyName(state=initialState,action){ 
    switch(action.type){
        case CHANGENAME:
            return action.data
        default:
            return state
    }
}
```


::right::

store.js
```js
const store = createStore(modifyName);
```
component
```js
 connect(state => ({ lastname:modifyName.name}),
    {changeNameCreater}
)(Component)
```

![Local Image](/images/redux.webp)

<!--

-->
