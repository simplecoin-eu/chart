### Get Started

Insert the following snippet in the place where you would like to display chart: 

```html
<div id="simplecoin-chart"></div>
<script>
    (function (s, i, m, p, l, e) {
        SimpleCoin = s.SimpleCoin || {};
        SimpleCoin.Widgets = SimpleCoin.Widgets || {};
        SimpleCoin.Widgets.Chart = SimpleCoin.Widgets.Chart || [];
        SimpleCoin.Widgets.Chart.push({
            id: 'simplecoin-chart',
            width: 1200,
            height: 650,
            fromCurrency: 'EUR',
            toCurrency: 'BTC',
        });
        l = i.createElement(p);l.src = m;l.async = 1;e = i.getElementsByTagName(p)[0];e.parentNode.append(l);
    })(window, document, 'https://cdn.simplecoin.ru/chart/launcher.js', 'script');
</script>
```


**Available options**:

| Option name   | Type                  | Description |
|---------------|-----------------------|-------------|
| id            | `string`              | HTML element selector `id` where to mount chart. |
| width         | `integer`/`string`    | Iframe width in px or other CSS supported units. |
| height        | `integer`/`string`    | iframe height in px or other CSS supported units. |
| fromCurrency  | `string`              | This currency would preselected on "from" side. Should be ISO 4217 compatible, e.g. BTC. |
| toCurrency    | `string`              | This currency would preselected on "to" side. Should be ISO 4217 compatible, e.g. EUR. |
| affiliateId   | `integer`             | Your affiliate ID. This ID would be used on every URL inside chart to make  |
| styleUrl      | `string`              | URL to CSS which would be embedded. It can be used to customize theming.
