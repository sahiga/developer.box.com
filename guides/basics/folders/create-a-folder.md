---
rank: 1
tag: folders
related_endpoints:
  - post_folders_id
related_guides:
  - basics/folders/-folder
  - basics/folders/copy-a-folder
required_guides: []
alias_paths: []
id: basics/folders/create-a-folder
cId: basics
scId: basics/folders
isIndex: false
---
# フォルダの作成

Box上でフォルダを作成するには、新しいフォルダの`name`と、新しいフォルダの作成先になる`parent`フォルダの`id`をAPIに渡す必要があります。

<Samples id="post_folders">

</Samples>

<Message>

# 名前に関する制約事項

ファイル名にはいくつかの制約事項があります。印字不可能なASCII文字を含む名前、スラッシュおよびバックスラッシュ(`/`、`\`)を含む名前、末尾にスペースを含む名前は禁止されています。

また、`.`および`..`は予約済みの名前であるため、使用できません。

</Message>
