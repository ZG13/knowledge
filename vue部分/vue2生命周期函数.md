### beforCreate
实例初始化之后，组件被创建初期，这个时候el，data，message 等都没有被初始化
### created
实例创建完成，data，methods等已经被初始化，但是dom还未生成，$el属性还不存在
### beforeMount
挂载初始之前，完成 el 初始化，render被初次调用
### mounted
完成挂载，可以对dom进行操作
### beforeUpdate

### updated

### activated
配合keep-alive使用
组件激活时调用
### deactivated
配合keep-alive使用
组件停用时调用
### beforeDestroy
实例销毁前调用，清理定时器
### destroyed
实例销毁后调用
