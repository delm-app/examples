# Custom Widget #4

This is the code for the widget available at [https://demo.delm.io/products/custom-widget-4](https://demo.delm.io/products/custom-widget-4).

## Date formats

Change the date formats of your widget:

| Field               | Value                |
| ------------------- | -------------------- |
| Date range earliest | `{dddd}, {MMM} {DD}` |
| Date range latest   | `{dddd}, {MMM} {DD}` |
| Single date         | `{dddd}, {MMM} {DD}` |

## {order_deadline} placeholder content

```html
<style>
  .delm-visual-countdown {
    display: flex;
    line-height: 1;
    margin-top: 6px;
  }
  .delm-visual-countdown > div:not(.delm-visual-countdown__divider) {
    display: flex;
    height: 64px;
    flex: 1 1 0;
    flex-direction: column;
    justify-content: center;
    position: relative;
    background-color: #f9f9f9;
    border-radius: 6px;
    text-align: center;
    border: solid 1px #ddd;
  }
  .delm-visual-countdown__count {
    display: block;
    margin-bottom: 4px;
    color: #4271FD;
    font-size: 26px;
  }
  .delm-visual-countdown__label {
    font-size: 12px;
    text-transform: uppercase;
  }
  .delm-visual-countdown__divider {
    display: flex;
    align-items: center;
    color: #4271FD;
    font-size: 26px;
    margin: 0 6px;
  }
</style>

Order within:
<div class="delm-visual-countdown">{countdown}</div>
```

## {countdown} placeholder settings

| Field                | Value                                                                                                                    |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Day (singular)       | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Days</div></div>` |
| Days (plural)        | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Days</div></div>` |
| Hour (singular)      | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Hrs</div></div>`  |
| Hours (plural)       | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Hrs</div></div>`  |
| Minute (singular)    | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Mins</div></div>` |
| Minutes (plural)     | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Mins</div></div>` |
| Seconds              | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Secs</div></div>` |
| Words connector      | `<div class="delm-visual-countdown__divider">:</div>`                                                                    |
| Last words connector | `<div class="delm-visual-countdown__divider">:</div>`                                                                    |
| Show seconds         | `999`                                                                                                                    |
| Show leading zeros   | `Yes`                                                                                                                    |
| Show zero values     | `Yes`                                                                                                                    |
