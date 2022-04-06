# mobx
<br>

store
```js
class addressStore {
  @observable modalVisible = false;
  @computed get validationAddress() {
    return this.selectListValidationOption === 'originalAddress'
  }
  @action.bound
  setModalVisible(data) {
    this.modalVisible = data;
  }
}
```
component
```js
@inject('loginStore')
@seoHoc('Account pet')
@observer
class Pet extends React.Component {}
```