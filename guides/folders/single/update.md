---
rank: 2
related_endpoints:
  - put_folders_id
related_guides:
  - folders/single/update
required_guides:
  - folders/single/create
related_resources:
  - folder
alias_paths: []
cId: folders
scId: folders/single
id: folders/single/update
isIndex: false
---
# Update Folder

To update a folder in Box you will need to call the following API.

<Samples id="put_folders_id">

</Samples>

## 名前に関する制約事項

ファイル名にはいくつかの制約事項があります。印字不可能なASCII文字を含む名前、スラッシュおよびバックスラッシュ(`/`、`\`)を含む名前、末尾にスペースを含む名前は禁止されています。

また、`.`および`..`は予約済みの名前であるため、使用できません。

## Timeout

Timeout for this operation is 60 seconds. The operation will complete
after a `HTTP 503` has been returned.
