## `Pipeline.Downloader` 类型



模块: [cc](../modules/cc.md)
父模块: [cc](../modules/cc.md)


The downloader pipe, it can download several types of files:
1. Text
2. Image
3. Script
4. Audio
5. Assets
All unknown type will be downloaded as plain text.
You can pass custom supported types in the constructor.


### 索引



##### 方法

  - [`constructor`](#constructor) Constructor of Downloader, you can pass custom supported types.
  - [`addHandlers`](#addhandlers) Add custom supported types handler or modify existing type handler.
  - [`loadSubpackage`](#loadsubpackage) 通过子包名加载子包代码。



### Details




<!-- Method Block -->
#### 方法


##### constructor

Constructor of Downloader, you can pass custom supported types.

| meta | description |
|------|-------------|
| 定义于 | [cocos2d/core/load-pipeline/downloader.js:270](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L270) |

###### 参数列表
- `extMap` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Custom supported types with corresponded handler

##### 示例

```js
var downloader = new Downloader({
     // This will match all url with `.scene` extension or all url with `scene` type
     'scene' : function (url, callback) {}
 });
```

##### addHandlers

Add custom supported types handler or modify existing type handler.

| meta | description |
|------|-------------|
| 定义于 | [cocos2d/core/load-pipeline/downloader.js:295](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L295) |

###### 参数列表
- `extMap` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Object" class="crosslink external" target="_blank">Object</a> Custom supported types with corresponded handler


##### loadSubpackage

通过子包名加载子包代码。

| meta | description |
|------|-------------|
| 定义于 | [cocos2d/core/load-pipeline/downloader.js:353](https://github.com/cocos-creator/engine/blob/d6ec4c03aa86f40af14d21ef9f059fed5e540c58/cocos2d/core/load-pipeline/downloader.js#L353) |

###### 参数列表
- `name` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/String" class="crosslink external" target="_blank">String</a> Subpackage name
- `completeCallback` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Function" class="crosslink external" target="_blank">Function</a> Callback invoked when subpackage loaded
	- `error` <a href="https://developer.mozilla.org/en/JavaScript/Reference/Global_Objects/Error" class="crosslink external" target="_blank">Error</a> error information



