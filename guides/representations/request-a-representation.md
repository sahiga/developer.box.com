---
rank: 2
related_endpoints:
  - get_files_id
related_guides:
  - representations/download-a-representation
  - representations/supported-file-types
  - representations/x-rep-hints
required_guides:
  - representations/list-all-representations
alias_paths: []
id: representations/request-a-representation
cId: representations
scId: null
isIndex: false
---

# Request a desired representation

To select a specific representation call the [`GET /files/:id`][get_files_id]
endpoint with a `X-Rep-Hints`-header defining the required representation format.

```sh
curl https://api.box.com/2.0/files/123?fields=representations \
  -H "X-Rep-Hints: [pdf]" \
  -H "Authorization: Bearer <AccessToken>"


```

## Requesting representations with multiple dimensions

Some formats will require the `dimensions` to be passed in to select a
specific size. This can be achieved by appending the `dimensions` to the
header.

```sh
curl https://api.box.com/2.0/files/123?fields=representations \
  -H "X-Rep-Hints: [jpg?dimensions=94x94]" \
  -H "Authorization: Bearer <AccessToken>"


```

## Requesting multiple representations

Multiple representations can be fetched by chaining the different
types in the `X-Rep-Hints`-header.

```sh
curl https://api.box.com/2.0/files/123?fields=representations \
  -H "X-Rep-Hints: [pdf][jpg?dimensions=94x94]" \
  -H "Authorization: Bearer <AccessToken>"


```

## API Response

This API call will result in one or more representations with a `url_template`
value that includes a `{+asset_path}` value.

```json
{
  "etag": "1",
  "id": "123",
  "representations": {
    "entries": [
      {
        "content": {
          "url_template": "https://dl.boxcloud.com/api/2.0/internal_files/123/versions/345/representations/pdf/content/{+asset_path}"
        },
        "info": {
          "url": "https://api.box.com/2.0/internal_files/123/versions/345/representations/pdf"
        },
        "properties": {},
        "representation": "pdf",
        "status": {
          "state": "success"
        }
      }
    ]
  },
  "type": "file"
}
```

<Message type='notice'>

The `url_template` in this response is an **opaque** URL. This URL format
might change over time and no assumptions should be made about its format
except for the presence of the `{+asset_path}` variable.

</Message>

[get_files_id]: (/reference/get-files-id/)