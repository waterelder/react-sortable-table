## Sortable Table in React.js

[![npm version](https://badge.fury.io/js/react-sortable-table.svg)](http://badge.fury.io/js/react-sortable-table)

### INSTALL
`npm install react-sortable-table`

### USING
```
@sample.jsx

var React = require("react");

var SortableTable = require("../../react-sortable-table");

var data = [
    { id: 3, name: "Satoshi", class: "B" },
    { id: 1, name: "Taro", class: "A" },
    { id: 2, name: "Ken", class: "A" },
    { id: 4, name: "Masaru", class: "C" }
];

var columns = [
    { header: "ID", key: "id", defaultSorting: "ASC", headerStyle: {fontSize: "15px", backgroundColor: "#FFDAB9" }, dataStyle: {fontSi\
ze: "15px", backgroundColor: "#FFDAB9"} },
    { header: "NAME", key: "name", headerStyle: {fontSize: "15px"} },
    { header: "CLASS", key: "class", headerStyle: {fontSize: "15px"} }
];

var style = {
    backgroundColor: "#eee"
};

var style = {
    backgroundColor: "#eee"
};

var iconStyle = {
    color: "#aaa",
    paddingLeft: "5px",
    paddingRIght: "5px"
};

React.render(<SortableTable data={data} columns={columns} style={style} iconStyle={iconStyle} />, document.body);
```

### PropTypes
- data: React.PropTypes.array.isRequired
- columns: React.PropTypes.array.isRequired
