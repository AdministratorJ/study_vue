```javascript
handleEdit(todo){
    // 显示input框
    todo.showInput = true
    // 获取input框的焦点。在这里没有用，虽然数据改了，但是没有去更新DOM。方法执行完再去更新。
    this.$refs.showinput.focus()

    // 可以使用这个$nextTick 表示下一次更新完DOM后执行。
    this.$nextTick(function(){
        this.$refs.showinput.focus()
    })
}
```
