文档结构修改中, 之前版本请戳[这里](https://github.com/xswei/d3js_doc/tree/master/d3js_doc_old)

# D3: Data-Driven Documents

<a href="https://d3js.org"><img src="https://d3js.org/logo.svg" align="left" hspace="10" vspace="20"></a>

**D3** (或者叫**D3.js**)是一个基于web标准的JavaScript可视化库。D3可以借助SVG,Canvas以及HTML将你的数据生动的展现出来。D3结合了强大的可视化交互技术以及数据驱动DOM的技术结合起来，让你可以借助于现代浏览器的强大功能自由的对数据进行可视化。


## 资源

* [API 参考](https://github.com/d3/d3/blob/master/API.md)
* [发布说明](https://github.com/d3/d3/releases)
* [画廊](https://github.com/d3/d3/wiki/Gallery)
* [例子](https://bl.ocks.org/mbostock)
* [Wiki](https://github.com/d3/d3/wiki)

## 安装

如果使用`npm`，则可以通过`npm install d3`来安装。此外还可以下载[最新版](https://unpkg.com/d3/build/)，最新版支持AMD、CommonJS以及vanilla环境。你也可以直接从 [d3js.org](https://d3js.org), [CDNJS](https://cdnjs.com/libraries/d3), 或者 [unpkg](https://unpkg.com/d3/) 加载。比如:

```html
<script src="https://d3js.org/d3.v4.js"></script>
```

压缩版:

```html
<script src="https://d3js.org/d3.v4.min.js"></script>
```

你也可以单独使用d3中的某个模块，比如单独使用[d3-selection](https://github.com/d3/d3-selection)：

```html
<script src="https://d3js.org/d3-selection.v1.min.js"></script>

```

如果要使用某个固定的版本，则考虑[CNDJS](https://cdnjs.com/libraries/d3) 或[ unpkg](https://unpkg.com/d3/)

D3基于[ES2015 modules](http://www.2ality.com/2014/09/es6-modules-final.html)开发。 可以使用Roolup, webpack或者其他你偏爱的打包工具进行构建。在一个符合ES2015的应用中导入D3或者D3的某些模块:

```js
import {scaleLinear} from "d3-scale";
```

或者导入D3的全部功能并且设置命名空间 (这里是 `d3`):

```js
import * as d3 from "d3";
```

在Node环境中:

```js
var d3 = require("d3");
```

你也可以导入多个模块然后将这些模块集合到`d3`对象中，此时使用 [Object.assign](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/assign):

```js
var d3 = Object.assign({}, require("d3-format"), require("d3-geo"), require("d3-geo-projection"));
```
