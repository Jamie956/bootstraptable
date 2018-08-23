### bootstrapTable 的配置

```
表头
columns
表格数据
data
表格风格
classes
showRefresh: true,//是否显示 刷新按钮
toolbar: "#toolbar",
showToggle: "true",//是否显示 切换试图
showColumns: "true",//是否显示 内容列下拉框
queryParams: "queryParams",//请求服务器数据时，可以通过重写参数的方式添加一些额外的参数
responseHandler: "responseHandler",//加载服务器数据之前的处理程序，可以用来格式化数据。参数
pagination: "true",//是否分页显示
search: "true",//是否支持搜索
pageList: "[5, 10, 20, 50, 100, 200]",//页面数据条数
url:"/examples/bootstrap_table/data",//请求数据
sidePagination: "server",//server or client 分页
onClickRow: function (row) {}　//单机一行的回调函数
```

### columns

```
field
title
格式化单元格内容
formatter
sortable: 'true',//是否可搜索
visible: true,//是否可见
```
