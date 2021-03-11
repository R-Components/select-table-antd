# select-table-antd

> 支持 antd checkbox 的滚动加载表格组件，适用于表格数据量大 不用翻页 支持选择的场景


## Install

```bash
npm install --save select-table-antd
```

## Usage

```jsx
import React, { Component } from 'react'

import SelectableTable from 'select-table-antd'

class Example extends Component {
  const columns = [

  ]
  onSelectRows = () => {

  }
  render () {
    return (
      <SelectableTable
        width={220}
        height={420}
        selectable
        columns={columns}
        className=''
        data={[]}
        rowKey="id"
        onRowSelect={this.onSelectRows}
        onSelectedRowsChange={(r) => {console.log(r, 'rrr'); this.setState({ selectedRowKeys: r})}}

        allRows={selectedRowKeys}

        headerRenderer={null}
      />
    )
  }
}
```

## License

MIT © [Go7hic](https://github.com/Go7hic)
