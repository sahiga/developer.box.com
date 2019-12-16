---
rank: 2
related_endpoints:
  - put_files_id
related_guides:
  - shared-links/create
  - shared-links/remove
  - shared-links/find-for-item
related_pages: []
required_guides: []
related_resources: []
alias_paths: []
cId: shared-links
scId: null
id: shared-links/update
isIndex: false
---
# Update Shared Link

A shared link may be updated from a resource by calling the [update file](endpoint://put_files_id) or [update folder](endpoint://put_folders_id) endpoint, specifying the ID of the resource to update with the new shared link values. See the [create shared link](guide://shared-links/create) guide for all available parameters.

<Message type="notice">

If you update the shared link settings, the new settings will apply to any users who already have the URL.

</Message>

## Update Shared Link on File

To update a shared link on a file, specify the ID of the file with any optional shared link parameters.

<Samples id="put_files_id_shared_link_create">

</Samples>

## Update Shared Link on Folder

To update a shared link on a folder, specify the ID of the folder with any optional shared link parameters.

<Samples id="put_folders_id_shared_link_create">

</Samples>
