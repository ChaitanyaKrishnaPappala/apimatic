# Collection Curator

```ts
const collectionCuratorController = new CollectionCuratorController(client);
```

## Class Name

`CollectionCuratorController`


# Create a Collection

Creating a collection for Collection Curator

```ts
async createACollection(
  body: unknown,
  requestOptions?: RequestOptions
): Promise<ApiResponse<unknown>>
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | `unknown` | Body, Required | body |
| `requestOptions` | `RequestOptions \| undefined` | Optional | Pass additional request options. |

## Response Type

`unknown`

## Example Usage

```ts
const body = '{"userID":"4a52606a-d061-4104-9c8c-1e66cedb6529","queryTerm":"styleColor","skus":[{"styleNumber":"K7690","skuName":"BLM","styleGroup":"Backpack","skuTarget":"1233"},{"styleNumber":"K7690","skuName":"CU3","styleGroup":"test no group","skuTarget":"5"},{"styleNumber":"K7676","skuName":"CU3","styleGroup":"test2","skuTarget":"4"},{"styleNumber":"K7485","skuName":"Y29","styleGroup":"Tote","skuTarget":"34545"},{"styleNumber":"K7484","skuName":"TU7","styleGroup":"","skuTarget":""},{"styleNumber":"K4366","skuName":"REM","styleGroup":"","skuTarget":""},{"styleNumber":"","skuName":"","styleGroup":"Hobo 12","skuTarget":"122"},{"styleNumber":"","skuName":"","styleGroup":"Crossbo1dy","skuTarget":"122"},{"styleNumber":"","skuName":"","styleGroup":"Belt bag123","skuTarget":"345"}],"season":"summer","year":"FY22","brand":"ks","title":"Test SKU Error 2","channel":"mainline"}';
try {
  const { result, ...httpResponse } = await collectionCuratorController.createACollection(body);
  // Get more response info...
  // const { statusCode, headers } = httpResponse;
} catch(error) {
  if (error instanceof ApiError) {
    const errors = error.result;
    // const { statusCode, headers } = error;
  }
}
```

## Example Response

```
"93eb353b-d6c9-4a33-858a-0d72bfd7c344"
```

