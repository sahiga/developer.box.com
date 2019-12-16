---
rank: 1
related_endpoints:
  - post_folders
related_guides:
  - folders/single/update
  - folders/single/copy
required_guides: []
related_resources:
  - folder
alias_paths: []
cId: folders
scId: folders/single
id: folders/single/create
isIndex: false
---
# Create Folder

Box上でフォルダを作成するには、新しいフォルダの`name`と、新しいフォルダの作成先になる`parent`フォルダの`id`をAPIに渡す必要があります。

<Samples id="post_folders">

</Samples>

<Message type="notice">

# 名前に関する制約事項

ファイル名にはいくつかの制約事項があります。印字不可能なASCII文字を含む名前、スラッシュおよびバックスラッシュ(`/`、`\`)を含む名前、末尾にスペースを含む名前は禁止されています。

Additionally, the names `.` and `..` are reserved names and therefore also prohibited.

</Message>
