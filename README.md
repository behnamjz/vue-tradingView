# vue-tradingView
> It's a Trading view chart component for Vue and Nuxt.

vue-tradingView is a dependency-free, lightweight vue component that can be overwrited by yourself.
It is support vue-ssr.

### How to use?
```bash
npm install vue-tradingView
```

### Example

```vue
<template>
  <vue-trading-view :options="chartOptions"></countup>
</template>

<script>
  import vuetradingView from 'vue-tradingView';
  export default {
    components: { countUp },
    data () {
      return {
        chartOptions: {
            theme: 'light',
            symbol: 'BTCUSDT',
            width: 980,
            height: 600,
            hide_top_toolbar: true,
            interval: 240 // thats mean's 4h //
        }
      }
    }
  }
</script>
```

### Options
|    Property    |    Description   |   type   |	default	|
| -----------------  | ---------------- | :--------: | :----------: |
| theme         | set theme for chart between 'light' and 'dark'  | String | light |
| symbol  | set symbol for chart | String | |
| hide_top_toolbar     | Hide Toolbar | Boolean | false |
| interval | set time-based bar interval (1m[1] - 1h[60] - 1D[D] - 1W[W] - 1Y[Y]) | String | D |
| allow_symbol_change | allow to change symbol | Boolean | true |
| callendar | show callendar | Boolean | false |
.
.
.

for more options can see [this page](https://www.tradingview.com/widget/advanced-chart/) for the TradingView Advanced Real-Time Chart API.

