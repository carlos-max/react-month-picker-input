React-Month-Picker-Input
====================

A month picker input and calendar for [React](http://facebook.github.io/react/index.html).


## API

| Name | Types | Default | Description |
|---|---|---|---|
| year | number | void | Preselect year in calendar |
| month | number (0..11) | void | Preselect month in calendar. If both year and month are specified then input field will be also prepopulated |
| inputProps | object | empty object | Input field props, only `id`, `name`, 'className' and 'disabled' are supported |
| onChange | Function: (maskedValue: string, year: number, month: number) => any | - | onChange callback, receives `maskedValue`, `year` and `month` (begins with 0) as arguments |

## Installation

```
npm install max-month-picker --save
```

## Usage

React-Month-Picker-Input generates an input field and year/month calendar opened on field focus.

```js
var MonthPickerInput = require('react-month-picker-input');
require('react-month-picker-input/dist/react-month-picker-input.css');

<MonthPickerInput
  id='string'
  className="form-control"
  value={new Date()}
  onChange={function(selectedYear, selectedMonth) {
    console.log(selectedYear, selectedMonth);
  }}
/>
```

## License

Copyright (c) [MIT](LICENSE) License.
