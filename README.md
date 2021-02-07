# node-red-contrib-excelsheets

## Overview

Features the ability to save data to multiple sheets. I found it wasn't supported in some of the other nodes already available.

To see an example, install the package, then in your Node-RED environment go to Import > Examples > node-red-contrib-excelsheets

Basic **msg** format is,

```
payload: [
    {
        header: {
            col1: "Column 1",
            col2: "Column 2",
            ...
        } ,
        items: [
            {
                col1: "data",
                col2: "data",
                ...
            }
        ] ,
        sheetName: "Sheet 1"
    } ,
    {header, items, sheetName} ,
    {header, items, sheetName} ,
    {header, items, sheetName} ,
    ...
] ,
filename: "output.xlsx"
```

## Change Log
* 1.0.0 - Original version, forked from "node-red-contrib-excel" and swapped out a different dependency.
* 1.0.1 - Cleanup.
* 1.0.2 - Cleanup and documentation.
* 1.0.3 - Cleanup and documentation.

## TODO
- [ ] Digging deeper into the dependencies, there's a really powerful package called "xlsx" [npmjs.com](https://www.npmjs.com/package/xlsx) that has a rich base of features, I would like to create a node that uses everything available.
- [ ] Come up with a few examples that do something more interesting