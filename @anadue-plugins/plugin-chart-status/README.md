## @anadue-plugins/plugin-chart-status

[![Version](https://img.shields.io/npm/v/@superset-ui/plugin-chart-status.svg?style=flat-square)](https://img.shields.io/npm/v/@superset-ui/plugin-chart-status.svg?style=flat-square)

This plugin provides Status for Superset.

### Usage

Configure `key`, which can be any `string`, and register the plugin. This `key` will be used to lookup this chart throughout the app.

```js
import StatusChartPlugin from '@anadue-plugins/plugin-chart-status';

new StatusChartPlugin()
  .configure({ key: 'nielsen-oss-status' })
  .register();
```

Then use it via `SuperChart`. See [storybook](https://apache-superset.github.io/superset-ui/?selectedKind=plugin-chart-status) for more details.

```js
<SuperChart
  chartType="anadue-oss-status"
  width={600}
  height={600}
  formData={...}
  queriesData={[{
    data: {...},
  }]}
/>
```
