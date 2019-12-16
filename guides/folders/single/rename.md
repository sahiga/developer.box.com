---
rank: 3
related_endpoints:
  - put_folders_id
related_guides:
  - folders/single/update
required_guides: []
related_resources:
  - folder
alias_paths: []
cId: folders
scId: folders/single
id: folders/single/rename
isIndex: false
---
# Rename Folder

To rename a folder in Box you will need to provide our API with a new `name` for the folder.

<Samples id="put_folders_id" variant="rename">

</Samples>

<Message type="notice">

# 名前に関する制約事項

ファイル名にはいくつかの制約事項があります。印字不可能なASCII文字を含む名前、スラッシュおよびバックスラッシュ(`/`、`\`)を含む名前、末尾にスペースを含む名前は禁止されています。

Additionally, the names `.` and `..` are reserved names and therefore also prohibited.

</Message>
