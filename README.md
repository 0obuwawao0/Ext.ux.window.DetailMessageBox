# Ext.ux.window.DetailMessageBox
带有可以折叠详细信息的对话框，该扩展组件是基于ExtJS5.1.1版本仿照MessageBox单例窗口编写。

## 部署扩展
将 `DetailMessageBox.js` 文件放于项目所在的 ExtJS 库目录
新建立 `ux/window` 即可

## 引入扩展
在对应的 `controller` 中使用 `requires` 将 `Ext.ux.window.DetailMessageBox` 类名引入：
```javascript

requires : [
  'Ext.ux.window.DetailMessageBox'
]

```

## 使用方法
因为该扩展定义的为单例窗口，在引入时就已实例化，所以在需要弹出详细对话框时可以直接使用别名 `Ext.ux.DetailMsg` 进行操作：

```javascript

Ext.ux.DetailMsg.show({
   title : '弹出窗口标题',
   icon : Ext.Msg.QUESTION,
   width : 300,
   msg : '弹出消息类容',
   bDetail : '弹出消息内容下方详细信息',
   buttons: Ext.Msg.OKCANCEL
})

```