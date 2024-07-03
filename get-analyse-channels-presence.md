[service-omnichannel](../../../../README.md) / [API](../README.md) / [Analyses](./README.md) / Get channels presence of an  analysis 

# Get channels presence of an analyse

Get channels presence of an  analysis 

```text
GET /analyses/:id/channels-presence
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
GET /analyses/665746252624a663d285deb0/channels-presence

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
      "channelName": "Paid Search",
      "presenceConversions": 2513
    },
    {
      "channelName": "Organic Search",
      "presenceConversions": 2896
    }
  ],
  "count": 2,
  "page": 1,
  "total": 11,
  "pageCount": 6
}
            

```