```javascript
Vue.set(vm.student, "sex", "男");
vm.$set(vm.student, "sex", "男");

new Vue({
    el: "#root",
    data: {
        student: {
            name: "gg",
        },
    },
    methods: {
        addSex() {
            Vue.set(this.student, "sex", "男");
            this.$set(this.stuednt, "sex", "男");
        },
    },
});
```
