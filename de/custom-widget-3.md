# Custom Widget #3

Dies ist der Code für das Widget, welches unter [https://demo.delm.io/de/products/custom-widget-3](https://demo.delm.io/de/products/custom-widget-3) verfügbar ist.

## Widget-Inhalt

Kopiere den folgenden HTML-Code in das Feld für den Widget-Inhalt:

```html
<style>
  .delm-custom-widget-3__timeline {
    display: flex;
    align-items: center;
    background-color: #fafafa;
    border: solid 1px #dddddd;
    border-radius: 4px;
    font-size: 14px;
    line-height: 1;
  }

  .delm-custom-widget-3__section {
    position: relative;
    width: calc(100%/3);
    padding: 10px 0;
    text-align: center;
    border-right: solid 1px #ddd;
  }

  .delm-custom-widget-3__section:not(:last-child):after {
    content: '';
    position: absolute;
    z-index: 1;
    top: 50%;
    right: 0;
    width: 12px;
    height: 12px;
    background-color: #fafafa;
    border: medium none;
    border-style: solid;
    border-color: rgba(34, 36, 38, .15);
    border-width: 0 1px 1px 0;
    -webkit-transform: translateY(-50%) translateX(50%) rotate(-45deg);
    transform: translateY(-50%) translateX(50%) rotate(-45deg);
  }

  .delm-custom-widget-3__section:last-child {
    border-right: 0;
  }

  .delm-custom-widget-3__icon {
    margin-bottom: 5px;
  }

  .delm-custom-widget-3__icon svg {
    width: 24px;
    height: 24px;
    fill: #222222;
  }

  .delm-custom-widget-3__date {
    margin-bottom: 5px;
    font-weight: 700;
  }
</style>

<div class="delm-custom-widget-3">
  <div style="margin-bottom: 10px;">
    <b>Lieferung nach <img src="https://flagcdn.com/16x12/{country_code_lower}.png" width="16" height="12" alt="{country_code_lower}" style="vertical-align: middle;"> {country_name} {delivery_date}.</b> {order_deadline}
  </div>
  <div class="delm-custom-widget-3__timeline">
    <div class="delm-custom-widget-3__section">
      <div class="delm-custom-widget-3__icon">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M19 3H18V1H16V3H8V1H6V3H5C3.9 3 3 3.9 3 5V19C3 20.11 3.9 21 5 21H19C20.11 21 21 20.11 21 19V5C21 3.9 20.11 3 19 3M19 19H5V9H19V19M5 7V5H19V7H5M10.56 17.46L16.5 11.53L15.43 10.47L10.56 15.34L8.45 13.23L7.39 14.29L10.56 17.46Z" />
        </svg>
      </div>
      <div class="delm-custom-widget-3__date">Heute</div>
      <div>Bestellt</div>
    </div>
    <div class="delm-custom-widget-3__section">
      <div class="delm-custom-widget-3__icon">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M.75 7.5H10.5L11.25 9H1.5L.75 7.5M1.75 10.5H11.5L12.25 12H2.5L1.75 10.5M18 18.5C18.83 18.5 19.5 17.83 19.5 17C19.5 16.17 18.83 15.5 18 15.5C17.17 15.5 16.5 16.17 16.5 17C16.5 17.83 17.17 18.5 18 18.5M19.5 9.5H17V12H21.46L19.5 9.5M8 18.5C8.83 18.5 9.5 17.83 9.5 17C9.5 16.17 8.83 15.5 8 15.5C7.17 15.5 6.5 16.17 6.5 17C6.5 17.83 7.17 18.5 8 18.5M20 8L23 12V17H21C21 18.66 19.66 20 18 20C16.34 20 15 18.66 15 17H11C11 18.66 9.65 20 8 20C6.34 20 5 18.66 5 17H3V13.5 13.5H5V15H5.76C6.31 14.39 7.11 14 8 14C8.89 14 9.69 14.39 10.24 15H15V6H3V6C3 4.89 3.89 4 5 4H17V8H20Z" />
        </svg>
      </div>
      <div class="delm-custom-widget-3__date">{shipping_date}</div>
      <div>Versendet</div>
    </div>
    <div class="delm-custom-widget-3__section">
      <div class="delm-custom-widget-3__icon">
        <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M2,10.96C1.5,10.68 1.35,10.07 1.63,9.59L3.13,7C3.24,6.8 3.41,6.66 3.6,6.58L11.43,2.18C11.59,2.06 11.79,2 12,2C12.21,2 12.41,2.06 12.57,2.18L20.47,6.62C20.66,6.72 20.82,6.88 20.91,7.08L22.36,9.6C22.64,10.08 22.47,10.69 22,10.96L21,11.54V16.5C21,16.88 20.79,17.21 20.47,17.38L12.57,21.82C12.41,21.94 12.21,22 12,22C11.79,22 11.59,21.94 11.43,21.82L3.53,17.38C3.21,17.21 3,16.88 3,16.5V10.96C2.7,11.13 2.32,11.14 2,10.96M12,4.15V4.15L12,10.85V10.85L17.96,7.5L12,4.15M5,15.91L11,19.29V12.58L5,9.21V15.91M19,15.91V12.69L14,15.59C13.67,15.77 13.3,15.76 13,15.6V19.29L19,15.91M13.85,13.36L20.13,9.73L19.55,8.72L13.27,12.35L13.85,13.36Z" />
        </svg>
      </div>
      <div class="delm-custom-widget-3__date">{delivery_date}</div>
      <div>Geliefert</div>
    </div>
  </div>
</div>
```

## Datumsformate

Ändere die Datumsformate deines Widgets:

| Feld                          | Wert                    |
| ----------------------------- | ----------------------- |
| Datumsbereich                 | `{earliest} – {latest}` |
| Datumsbereich frühestes Datum | `{D}. {MMM}`            |
| Datumsbereich spätestes Datum | `{D}. {MMM}`            |
| Einzelnes Datum               | `{D}. {MMM}`            |
| Morgen                        | `Morgen`                |
| Heute                         | `Heute`                 |
