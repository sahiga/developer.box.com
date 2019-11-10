---
rank: 50
related_endpoints: []
related_guides: []
required_guides: []
related_resources:
  - folder
  - folders
alias_paths:
  - /docs/work-with-folders
cId: folders
scId: null
id: folders
isIndex: true
---
# フォルダ

Creates a copy of a folder within a destination folder.

The original folder will not be changed.

## 非同期コピー

コピーされるフォルダに含まれる項目が500個以下の場合は、API呼び出しと同時にコピーが実行されます。呼び出しはコピー操作が完了するまで復帰しません。

コピー元のフォルダに500個を超える項目が含まれる場合は、非同期的にコピー操作が実行され、API呼び出しはコピー操作が完了していなくても直ちに復帰します。現時点では、コピー操作がいつ終了したのかを確認するAPIはありません。

## フォルダのロック

この操作の進行中は、ファイルツリーの一部がロックされます。ロックされるのは、主に元のフォルダとその子孫フォルダ、および宛先フォルダです。

操作の進行中は、ロックされているどのフォルダに対しても、他の移動、コピー、削除、または復元操作を実行できません。最も重要な点は、同じフォルダをフォルダツリーの2つの異なる部分に同時にコピーすることはできないということです。

## メタデータ

宛先フォルダのいずれかの親フォルダにメタデータカスケードポリシーが適用されている場合は、メタデータカスケード操作が非同期的に開始されます。

現時点では、この操作がいつ終了したのかを確認するAPIはありません。