---
rank: 4
related_endpoints:
  - get_files_id_content
related_guides:
  - downloads/file
  - uploads/direct/file
required_guides: []
related_resources: []
alias_paths:
  - /docs/download-all-files-from-a-folder-1
cId: downloads
scId: null
id: downloads/in-browser
isIndex: false
---
# Download in Browser

Sometimes an application wants to embed a file into a page as a HTML element. An
example would be when working with an audio player.

```html
<audio controls>
  <source src="..." type="audio/mp3">
</audio>
```

In this case, using the regular [durl][durl] does not work because the
`dl.boxcloud.com` domain does not support [cors][cors].

Instead an application can use the following format.

```sh
https://api.box.com/2.0/files/[FILE_ID]/content?access_token=[ACCESS_TOKEN]
```

<Message>

# CORS

For this to work the application needs to have the domain of the web site
hosting this file whitelisted in the [cors][cors].

</Message>

<Message>

# Downscope Token

Using this method would expose the Access Token to the end user, allowing them
to potentially use this token to do more than intended. For this reason we
recommend [downscoping][downscoping] this token accordingly.

</Message>

[durl]: g://downloads/get-url

[cors]: g://best-practices/cors

[downscoping]: g://authentication/access-tokens/downscope
