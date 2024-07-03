[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / get analyse conversions paths 

# Get client anlayse conversions paths

Get conversion paths for an analysis of client . 

```text
GET analyses/:id/conversion-paths
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
GET analyses/665746252624a663d285deb0/conversion-paths

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
  "data": [
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "path": " Direct",
      "nb_touchpoints": 1,
      "conversions": 1972,
      "CA": 4573829.251123
    },
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "path": " Paid Search",
      "nb_touchpoints": 1,
      "conversions": 232,
      "CA": 543112.642311
    },
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "path": " Email",
      "nb_touchpoints": 1,
      "conversions": 74,
      "CA": 192519.426396
    }
  ],
  "count": 3,
  "page": 1,
  "total": 8340,
  "pageCount": 2780
}
            

```
