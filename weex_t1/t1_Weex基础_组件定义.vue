<script>
	/*组件定义
定义组件是通过一组选项来描述一个组件。这组选项总是被赋值给 <script> 标签中的 module.exports 。
数据和方法
module.exports = {
  data: function () {
    return {x: 1, y: 2}
  },
  methods: {
    doThis: function () {...},
    doThat: function () {...}
  },
  event:{
	customtype1: function (e) {
      console.log(e.type, e.detail)
    }
  },
  init: function () {
    console.log('ViewModel constructor begins')
  },
  created: function () {
    console.log('Data observation finished')
  },
  ready: function () {
    console.log('Virtual DOM finished')
  }
}
data 选项是一个函数，它返回这个视图模型可监听的数据对象。
methods 是一个映射，其中包含所有视图模型的方法。
每个 data 或 method 属性将被代理到视图模型实例中。this.x 读写数据，this.doThis() 调用方法。
events 选项允许你在视图模型被创建时注册自定义事件。然后，它会监听这些类型的事件，并通过函数类型的值处理它们。
Weex 会把一个事件对象作为第一个参数传递给其绑定的事件，这个事件对象在 e.detail 中包含事件数据。
	*//*生命周期
Weex 视图模型现在支持生命周期内的钩子函数，这些钩子函数能被写为组件选项：
init: 在视图模型的构造函数开始调用时激活；
created: 当视图模型监听默认数据，但还未编译模板时激活；
ready: 当视图模型监听默认数据并且编译模板生成虚拟DOM后被激活。
	*/
</script>