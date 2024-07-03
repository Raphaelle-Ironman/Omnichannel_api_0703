[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Get channels attribution of an  analysis 

# Get analyse channels attribution

Obtain channel attribution from various models of an analysis. 

```text
GET /analyses/:id/channels-attribution
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
GET /analyses/665746252624a663d285deb0/channels-attribution

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
      "channelName": "Organic Video",
      "firstTouchConversions": "188",
      "lastTouchConversions": "132",
      "linearConversions": "34",
      "markovConversions": "97",
      "firstTouchValue": "141303",
      "lastTouchValue": "155685",
      "linearValue": "175396",
      "markovValue": "89805"
    },
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "channelName": "Organic Video",
      "firstTouchConversions": "188",
      "lastTouchConversions": "132",
      "linearConversions": "34",
      "markovConversions": "97",
      "firstTouchValue": "141303",
      "lastTouchValue": "155685",
      "linearValue": "175396",
      "markovValue": "89805"
    }
  ],
  "count": 2,
  "page": 1,
  "total": 8,
  "pageCount": 4
}
            

```
