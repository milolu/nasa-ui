# 日期最大跨度选择控件

|参数 | 说明 | 类型 | 默认值   |
|  -  |  -   |  -   |   - |
|range |  时间最大跨度，如果为数值，则代表前后跨度一致，如果为数组，range[0]为前段时间跨度，range[1]为后段时间跨度 | Number or Array | 必填|
|disabledDate | 不可点击日期 | Function | 默认为时间跨度之外不可选，如果定义此函数，函数的第二个参数为跨度之外不可选的时间段|
|... | 其余参数参照Antd RangePicker | ... | |

<br/>

## 基本使用

```jsx
import { RangePickerEx } from 'nasa-ui';

<h3>设置时间跨度20天</h3>
<RangePickerEx range={10}></RangePickerEx>
<h3>自定义前后跨度</h3>
<RangePickerEx range={[2, 10]}></RangePickerEx>
```