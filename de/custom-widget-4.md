# Custom Widget #4

Dies ist der Code für das Widget, welches unter [https://demo.delm.io/de/products/custom-widget-4](https://demo.delm.io/de/products/custom-widget-4) verfügbar ist.

## {order_deadline} Platzhalter-Inhalt

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

Bestellung innerhalb:
<div class="delm-visual-countdown">{countdown}</div>
```

## {countdown} Platzhalter-Einstellungen

| Feld                     | Wert                                                                                                                     |
| ------------------------ | ------------------------------------------------------------------------------------------------------------------------ |
| Tag (Einzahl)            | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Tage</div></div>` |
| Tage (Mehrzahl)          | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Tage</div></div>` |
| Stunde (Einzahl)         | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Std</div></div>`  |
| Stunden (Mehrzahl)       | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Std</div></div>`  |
| Minute (Einzahl)         | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Min</div></div>`  |
| Minuten (Mehrzahl)       | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Min</div></div>`  |
| Sekunden                 | `<div><div class="delm-visual-countdown__count">{count}</div><div class="delm-visual-countdown__label">Sek</div></div>`  |
| Wortverbindung           | `<div class="delm-visual-countdown__divider">:</div>`                                                                    |
| Letzte Wortverbindung    | `<div class="delm-visual-countdown__divider">:</div>`                                                                    |
| Sekunden anzeigen        | `999`                                                                                                                    |
| Führende Nullen anzeigen | `Ja`                                                                                                                     |
| Nullwerte anzeigen       | `Ja`                                                                                                                     |
