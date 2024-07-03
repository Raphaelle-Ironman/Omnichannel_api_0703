[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Get path distribution of an analysis

# Get path distribution of an analysis

Retrieve the number of conversions for mono- and multi-channel paths

```text
GET /analyses/:id/paths-distribution
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
GET /analyses/665746252624a663d285deb0/paths-distribution

{
  "user": {
    "id": "123-abc-456",
    "workspaces": ["fake-id24"]
  },
  "workspaceId": "fake-id24"
}
```

Response

```text
200
```

```json
{
  "data": {
    "mono": 5895,
    "multi": 14582
  },
  "count": 1,
  "page": 1,
  "total": 1,
  "pageCount": 1
}
            

```