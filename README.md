## Usage

```js
var Tabs = require('uxcore-tabs');
var TabPane = Tabs.TabPane;

var callback = function(key){

}

React.render(
  (
    <Tabs defaultActiveKey="2" onChange={callback}>
      <TabPane tab='tab 1' key="1">first</TabPane>
      <TabPane tab='tab 2' key="2">second</TabPane>
      <TabPane tab='tab 3' key="3">third</TabPane>
    </Tabs>
  ),
  document.getElementById('t2'));
```

## development
```shell
npm install
npm run dev
// nav to http://localhost:9090/example/
```

## API
### Tabs
|name|type|default|description|
|----|----|-------|-----------|
|activeKey |String| |current active tabPanel's key|
|defaultActiveKey|	String|	first active tabPanel's key|	initial active tabPanel's key if activeKey is absent|
|onChange|	Function|(key)		|called when tabPanel is changed|
|onTabClick|	Function|(key)		|called when tab is clicked|
|size|string|normal|set tab size:mini, normal, large|
|tabStyle|string|underline|set tab style: underline, line, topline, brick|

### TabPane
|name|type|default|description|
|----|----|-------|-----------|
|key| Object | |corresponding to activeKey|
|tab| String | |current tab's title corresponding to current tabPane|
