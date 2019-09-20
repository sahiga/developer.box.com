---
rank: 3
tag: folders
related_endpoints:
  - delete_folders_id
related_guides:
  - basics/folders/create-a-folder
required_guides:
  - basics/folders/create-a-folder
alias_paths: []
id: basics/folders/delete-a-folder
cId: basics
scId: basics/folders
isIndex: false
---
# フォルダの削除

Box上でフォルダを削除するには、削除するフォルダのIDをAPIに渡す必要があります。

<Samples id="delete_folders_id">

</Samples>

<Message>

# 空でないフォルダの削除

フォルダを削除するときに`recursive`パラメータを渡すと、空でないフォルダも強制的に削除できます。その場合は、サブフォルダを含め、フォルダ内のすべての項目が削除されます。

</Message>
