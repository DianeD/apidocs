# Create version

Use this API to create a new version.
### Prerequisites
The following **scopes** are required to execute this API: 
### HTTP request
<!-- { "blockType": "ignored" } -->
```http
POST /drive/root/versions
POST /drive/items/<id>/versions
POST /drives/<id>/root/versions

```
### Request headers
| Name       | Type | Description|
|:---------------|:--------|:----------|
| X-Sample-Header  | string  | Sample HTTP header. Update accordingly or remove if not needed|

### Request body
In the request body, supply a JSON representation of [item](../resources/item.md) object.


### Response
If successful, this method returns `201, Created` response code and [item](../resources/item.md) object in the response body.

### Example
##### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_item_from_item"
}-->
```http
POST https://graph.microsoft.com/v1.0/drive/root
```
In the request body, supply a JSON representation of [item](../resources/item.md) object.
##### Response
Here is an example of the response.
<!-- {
  "blockType": "response",
  "truncated": false,
  "@odata.type": "microsoft.graph.item"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 3179

{
  "content": "content-value",
  "createdBy": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  },
  "createdDateTime": "datetime-value",
  "cTag": "cTag-value",
  "description": "description-value",
  "eTag": "eTag-value",
  "id": "id-value",
  "lastModifiedBy": {
    "application": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "device": {
      "displayName": "displayName-value",
      "id": "id-value"
    },
    "user": {
      "displayName": "displayName-value",
      "id": "id-value"
    }
  },
  "lastModifiedDateTime": "datetime-value",
  "name": "name-value",
  "parentReference": {
    "driveId": "driveId-value",
    "id": "id-value",
    "path": "path-value"
  },
  "size": 99,
  "webDavUrl": "webDavUrl-value",
  "webUrl": "webUrl-value",
  "audio": {
    "album": "album-value",
    "albumArtist": "albumArtist-value",
    "artist": "artist-value",
    "bitrate": 99,
    "composers": "composers-value",
    "copyright": "copyright-value",
    "disc": 99,
    "discCount": 99,
    "duration": 99,
    "genre": "genre-value",
    "hasDrm": true,
    "isVariableBitrate": true,
    "title": "title-value",
    "track": 99,
    "trackCount": 99,
    "year": 99
  },
  "deleted": {
    "state": "state-value"
  },
  "file": {
    "hashes": {
      "crc32Hash": "crc32Hash-value",
      "sha1Hash": "sha1Hash-value"
    },
    "mimeType": "mimeType-value"
  },
  "fileSystemInfo": {
    "createdDateTime": "datetime-value",
    "lastModifiedDateTime": "datetime-value"
  },
  "folder": {
    "childCount": 99
  },
  "image": {
    "height": 99,
    "width": 99
  },
  "location": {
    "altitude": 99,
    "latitude": 99,
    "longitude": 99
  },
  "openWith": {
    "web": {
      "app": {
        "displayName": "displayName-value",
        "id": "id-value"
      },
      "viewUrl": "viewUrl-value",
      "editUrl": "editUrl-value",
      "viewPostParameters": "viewPostParameters-value",
      "editPostParameters": "editPostParameters-value"
    },
    "webEmbedded": {
      "app": {
        "displayName": "displayName-value",
        "id": "id-value"
      },
      "viewUrl": "viewUrl-value",
      "editUrl": "editUrl-value",
      "viewPostParameters": "viewPostParameters-value",
      "editPostParameters": "editPostParameters-value"
    }
  },
  "photo": {
    "height": 99,
    "width": 99,
    "id": "id-value"
  },
  "searchResult": {
    "onClickTelemetryUrl": "onClickTelemetryUrl-value"
  },
  "shared": {
    "owner": {
      "application": {
        "displayName": "displayName-value",
        "id": "id-value"
      },
      "device": {
        "displayName": "displayName-value",
        "id": "id-value"
      },
      "user": {
        "displayName": "displayName-value",
        "id": "id-value"
      }
    },
    "scope": "scope-value"
  },
  "specialFolder": {
    "name": "name-value"
  },
  "video": {
    "bitrate": 99,
    "duration": 99,
    "height": 99,
    "width": 99
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create version",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->