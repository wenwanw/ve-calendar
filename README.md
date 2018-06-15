# ve-calendar

> This is a vue 2.0 based calendar component
>
<p align="center">
   <a href="https://www.npmjs.com/package/ve-calendar"><img src="https://img.shields.io/npm/v/ve-calendar.svg?style=flat " alt="npm"></a>
   <a href="https://www.npmjs.com/package/ve-calendar"><img src="https://img.shields.io/npm/dm/ve-calendar.svg?style=flat " alt="npm"></a>
 </p>
 
[Chinese document](./README.ZH.MD)

[English](./README.MD)

# Current function:
>1, display the lunar calendar, solar terms, festivals before 2050
>
> 2, can specify the maximum number of selected dates
>
>3, available slots custom date number, lunar calendar, event area


## Quick Start

### The first step:
``` sh
Npm install ve-calendar --save
```
### The second step, on your vue page
```js
Import veCalendar from "ve-calendar";

// in your vue <script>
Export default {
    Components: {
        veCalendar
    }
}
```

### The third step, loading the template:
``` html
<veCalendar v-model="selectDateList"></veCalendar>

```


## props parameter
Parameter Name | Type | Default | Description
---- | --- | --- | ---
Value | array | none | v-model binding value, is the current selected date list
Activate-date | object | date of the year | contains two values ​​year current year, month current month
Most-choice | number | 0 | up to choose the number of days, 0 infinity
Cross-month | boolean | false | whether to allow cross-month selection



## event
Name | Parameter | Description
---- | --- | ---
Refresh-calendar | None | Trigger/change activation year when switching calendars
Change | selectedDate/array | Fired when the selected date changes, the parameter is the list of currently selected dates (string)


## Preview
![Alt ​​text](./images/demo.png)


## License

[MIT] (https://github.com/pcloth/ve-calendar/blob/master/LICENSE)