[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Get channels summary of an  analysis 

# Get cliet analyse channels summary

Get channels summary of an  analysis . 

```text
GET /analyses/:id/channels-summary
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
GET /analyses/665746252624a663d285deb0/channels-summary

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
      "channelName": "Paid Search",
      "initiatorConversions": 1356,
      "assistantConversions": 1459,
      "finisherConversions": 638,
      "autonomousConversions": 424,
      "presenceConversions": 2513,
      "role": "assistant"
    },
    {
      "workspaceId": 1301,
      "analyseId": "fB1t5X73re5V991OVGus",
      "channelName": "Organic Search",
      "initiatorConversions": 1198,
      "assistantConversions": 2860,
      "finisherConversions": 1770,
      "autonomousConversions": 1185,
      "presenceConversions": 2896,
      "role": "assistant"
    }
  ],
  "count": 2,
  "page": 1,
  "total": 11,
  "pageCount": 6
}
            

```
