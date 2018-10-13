1.v-model
===
v-model的双向数据绑定可以说是Vue中类似于v-on（@）/v-bind（:）的一个“语法糖”  
以input元素为例 
```
<input v-model = " name ">
```
实际是这样实现的
```
<input v-bind:value=" name " v-on:input = "name = $event.target.value">
```
