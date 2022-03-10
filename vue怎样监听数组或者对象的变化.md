数组监听变化时不会监听索引变化
如friends:[{name:'gg'},{name:'hh'}] 
this.friends[0] = {name:'jj'} 数据会改，但是数据改变不会被监测到
Vue的geter和seter没有friednds[0]所以变化不会是响应式的数据。
但是有对friends的geter和seter，只有push，pop等数组方法才会引起响应式的变化
或者执行Vue.set(vm.friends,0,{name:'jj'})