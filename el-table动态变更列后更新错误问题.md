## el-table动态变更列后更新错误问题

在`el-table-column`中加入属性`key`，切记不可使用`:key="math.random()"`，推荐使用`computed`计算特定值，如

```javascript
computed: {
  tableRowKey() 
    // tableRowsConfig 是外部配置table列的数组
    const {length = 0} = this.tableRowsConfig;
    return 'row' + length
  }
},
```

