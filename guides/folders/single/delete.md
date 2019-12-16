---
rank: 6
related_endpoints:
  - delete_folders_id
related_guides:
  - folders/single/create
required_guides:
  - folders/single/create
alias_paths: []
related_resources:
  - folder
cId: folders
scId: folders/single
id: folders/single/delete
isIndex: false
---
# Delete Folder

Box上でフォルダを削除するには、削除するフォルダのIDをAPIに渡す必要があります。

<Samples id="delete_folders_id">

</Samples>

## 空でないフォルダの削除

フォルダを削除するときに`recursive`パラメータを渡すと、空でないフォルダも強制的に削除できます。その場合は、サブフォルダを含め、フォルダ内のすべての項目が削除されます。

## Recursive deletion

This API returns an error if the folder is not empty. You can use the `recursive` query parameter to force this operation to recursively delete the folder and all of its contents.

## フォルダのロック

The enterprise settings determine whether the folder will be permanently deleted from Box or moved to the trash.

During this operation, part of the file tree will be locked, mainly the source folder and all of its descendants.

For the duration of the operation, no other move, copy, delete, or restore operation can performed on any of the locked folders.

## Timeout

Timeout for this operation is 60 seconds. The operation will include after a `HTTP 503` has been returned.
