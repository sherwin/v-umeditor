# v-ueditor

> UMeditor 1.2.2 的Vue版本。

> 由于 1.2.3版本 无法选择字体和段落，目前使用1.2.2版本

[完整DEMO](http://assets.dxycdn.com/gitrepo/dxy-vue-ueditor/static/index.html?dsfg)

[DEMO](http://gitlab.dxy.net/biz-developer-f2e/dxy-vue-ueditor/blob/master/src/views/index.vue)

[仓库地址](http://gitlab.dxy.net/biz-developer-f2e/dxy-vue-ueditor)

## 安装

```js
npm i @dxy/v-ueditor -S
```
### 全局引用

```js
import vUeditor from '@dxy/v-ueditor'

Vue.use(vUeditor)
```

### 在组件内引用

```js
import vUeditor from '@dxy/v-ueditor'

components: {
  vUeditor
}
```

## 使用

```vue
<v-ueditor
  :config="config"
  @ready="ueditorReady"
></v-ueditor>
```

## props

| 字段     | 必填 | 类型    | 默认值 | 描述                                                          |
|:---------|:-----|:--------|:-------|:--------------------------------------------------------------|
| id       | 是   | String  | 无     | 当前编辑器 id                                                 |
| config   | 否   | Object  | {}     | 配置参数，详细参考 http://fex.baidu.com/ueditor/#start-config |
| newstyle | 否   | Boolean | true   | 是否使用新样式                                                |


## Events

| 字段  | 描述                                                                                                 | return |
|:------|:-----------------------------------------------------------------------------------------------------|:-------|
| ready | UEditor初始化后返回UEditor实例对象，可以调用实例方法，文档： http://ueditor.baidu.com/doc/#UE.Editor | UE实例 |

或者

```js
// 获取实例
window.UM.getEditor(id)
```
