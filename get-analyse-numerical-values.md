[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Get numerical values of an analysis

# Get numerical values of an analysis

Retrieve the numerical values for turnover, conversions, and number of paths of an analysis.

```text
GET /analyses/:id/numerical-values
```

## Body

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `user`         | The client's user information                       |
| `workspaceId`  | The current workspaceId                             |


## Parameters

| Name           | Description                                         |
|----------------|-----------------------------------------------------|
| `id`           | analyse id                                          |

## Example

```text
GET /analyses/665746252624a663d285deb0/numerical-values

{
  "user": {
    "id": "123-abc-456",
    "workspaces": ["fake-id24"]
  },
  "workspaceId": "fake-id24"s
}
```

Response

```text
200
```

```json
{
  "data": {
    "Nbpaths": 8340,
    "conversions": 31468,
    "turnover": 79232480.463792
  },
  "count": 1,
  "page": 1,
  "total": 1,
  "pageCount": 1
}
            

```