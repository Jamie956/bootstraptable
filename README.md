## bootstrapTable({})

```
columns
  field
  title
  formatter //处理columns
  sortable: 'true',//是否可搜索
  visible: true,//是否可见
  checkbox: true, //
data //数据
classes: 'table table-no-bordered'
showRefresh: true,//是否显示刷新按钮
toolbar: "#toolbar", //使用toolbar
showToggle: "true",//是否显示切换视图
showColumns: "true",//是否显示内容列下拉框
queryParams: "queryParams",//请求服务器数据时，重写参数添加额外参数
responseHandler: "responseHandler",//加载服务器数据之前的处理程序
pagination: "true",//是否分页显示
search: "true",//是否支持搜索
pageList: "[5, 10, 20, 50, 100, 200]",//页面数据条数
url:"/examples/bootstrap_table/data",//请求数据
sidePagination: "server",//server or client 分页
onClickRow: function (row) {}　//单击一行的回调函数
```

## Example
### columns config
```js
{
  field: 'price',
  title: 'Item Price',
  sortable: 'true',//是否可搜索
  visible: true,//是否可见
  formatter: function (value, row) {
    return 'ID: ' + value;
  }
}
```
### checkbox
```js
{
  field: 'state',
  title: 'State',
  checkbox: true,
  formatter: function (value, row, index) {
    if (index === 1) {
      return {
        disabled: true,
        checked: true
      }
    }
    return value;
  }
}
```

## $table.bootstrapTable('');
```js
$table.bootstrapTable('refresh');//刷新table
```














