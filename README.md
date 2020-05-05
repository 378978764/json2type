<div>
<svg width="370px" height="70px" viewBox="0 0 370 70" version="1.1" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
    <!-- Generator: Sketch 63.1 (92452) - https://sketch.com -->
    <title>画板</title>
    <desc>Created with Sketch.</desc>
    <g id="画板" stroke="none" stroke-width="1" fill="none" fill-rule="evenodd" font-family="RobotoMonoForPowerline-Thin, Roboto Mono Thin for Powerline" font-size="50" font-style="condensed" font-weight="300">
        <text id="JSON-To-Type" fill="#666666">
            <tspan x="4" y="52">JSON To Type</tspan>
        </text>
    </g>
</svg>
</div>

Convert json to golang, typescript, python3 type declaration.
## Usage
1、Install [tampermonkey](http://www.tampermonkey.net/).
2、Install [this script on greasyfork](https://greasyfork.org/zh-CN/scripts/402658-jsontogo).
2、Open browser console.
3、In the console, following commands are supported:

### **json text to golang type declaration**
input:
```javascript
document.jsonToGo('{"name":"user","age":18}')
```

output:
```golang
type AutoGenerated struct {
	Name string `json:"name"`
	Age int `json:"age"`
}
```

### **json text to typescript type declaration**
input:
```javascript
document.jsonToTs('{"name":"user","age":18}')
```

output:
```typescript
{
  name: string,
  age: number
}
```