
# Client Class Documentation

The following parameters are configurable for the API Client:

| Parameter | Type | Description |
|  --- | --- | --- |
| `xApiKey` | `string` | *Default*: `'VpWEGpl1w85F1lgHWE6Qw9gmUINSa5N26uBZvZrI'` |
| `authorization` | `string` |  |
| `environment` | Environment | The API environment. <br> **Default: `Environment.Develop`** |
| `timeout` | `number` | Timeout for API calls.<br>*Default*: `0` |
| `httpClientOptions` | `Partial<HttpClientOptions>` | Stable configurable http client options. |
| `unstableHttpClientOptions` | `any` | Unstable configurable http client options. |

The API client can be initialized as follows:

```ts
const client = new Client({
  xApiKey: 'VpWEGpl1w85F1lgHWE6Qw9gmUINSa5N26uBZvZrI',
  authorization: 'Authorization',
  timeout: 0,
  environment: Environment.Develop,
})
```

## Datalabs Client

The gateway for the SDK. This class acts as a factory for the Controllers and also holds the configuration of the SDK.

## Controllers

| Name | Description |
|  --- | --- |
| services | Gets ServicesController |
| collectionCurator | Gets CollectionCuratorController |

