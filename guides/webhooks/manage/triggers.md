---
rank: 6
related_endpoints:
  - post_webhooks
related_guides:
  - webhooks/manage/for-file
required_guides:
  - webhooks/manage/for-file
alias_paths: []
cId: webhooks
scId: webhooks/manage
id: webhooks/manage/triggers
isIndex: false
---
# Webhook Event Triggers

The following is a list of events that can trigger webhooks. Some events are only available for files, while others are only available for folders.

<!-- markdownlint-disable line-length -->

| イベント                        | トリガー                                                                                                                | ファイル? | フォルダ? |
| --------------------------- | ------------------------------------------------------------------------------------------------------------------- | ----- | ----- |
| `FILE.UPLOADED`             | A file is uploaded to this folder                                                                                   | いいえ   | はい    |
| `FILE.PREVIEWED`            | A file is previewed                                                                                                 | はい    | はい    |
| `FILE.DOWNLOADED`           | A file is downloaded                                                                                                | はい    | はい    |
| `FILE.TRASHED`              | A file is moved to the trash                                                                                        | はい    | はい    |
| `FILE.DELETED`              | A file is permanently deleted                                                                                       | はい    | はい    |
| `FILE.RESTORED`             | A file is restored from the trash                                                                                   | はい    | はい    |
| `FILE.COPIED`               | A file is copied                                                                                                    | はい    | はい    |
| `FILE.MOVED`                | A file is moved from one folder to another                                                                          | はい    | はい    |
| `FILE.LOCKED`               | A file is locked                                                                                                    | はい    | はい    |
| `FILE.UNLOCKED`             | A file is unlocked                                                                                                  | はい    | はい    |
| `FILE.RENAMED`              | A file was renamed.                                                                                                 | はい    | はい    |
| `COMMENT.CREATED`           | A comment object is created                                                                                         | はい    | はい    |
| `COMMENT.UPDATED`           | A comment object is edited                                                                                          | はい    | はい    |
| `COMMENT.DELETED`           | A comment object is removed                                                                                         | はい    | はい    |
| `TASK_ASSIGNMENT.CREATED`   | A task is created                                                                                                   | はい    | はい    |
| `TASK_ASSIGNMENT.UPDATED`   | A task assignment is changed                                                                                        | はい    | はい    |
| `METADATA_INSTANCE.CREATED` | A new metadata template instance is associated with a file or folder                                                | はい    | はい    |
| `METADATA_INSTANCE.UPDATED` | An attribute (value) is updated/deleted for an existing metadata template instance associated with a file or folder | はい    | はい    |
| `METADATA_INSTANCE.DELETED` | An existing metadata template instance associated with a file or folder is deleted                                  | はい    | はい    |
| `FOLDER.CREATED`            | A folder is created                                                                                                 | いいえ   | はい    |
| `FOLDER.RENAMED`            | A folder was renamed.                                                                                               | いいえ   | はい    |
| `FOLDER.DOWNLOADED`         | A folder is downloaded                                                                                              | いいえ   | はい    |
| `FOLDER.RESTORED`           | A folder is restored from the trash                                                                                 | いいえ   | はい    |
| `FOLDER.DELETED`            | A folder is permanently removed                                                                                     | いいえ   | はい    |
| `FOLDER.COPIED`             | A copy of a folder is made                                                                                          | いいえ   | はい    |
| `FOLDER.MOVED`              | A folder is moved to a different folder                                                                             | いいえ   | はい    |
| `FOLDER.TRASHED`            | A folder is moved to the trash                                                                                      | いいえ   | はい    |
| `WEBHOOK.DELETED`           | When a webhook is deleted                                                                                           | いいえ   | いいえ   |
| `COLLABORATION.CREATED`     | A collaboration is created                                                                                          | いいえ   | はい    |
| `COLLABORATION.ACCEPTED`    | A collaboration has been accepted                                                                                   | いいえ   | はい    |
| `COLLABORATION.REJECTED`    | A collaboration has been rejected                                                                                   | いいえ   | はい    |
| `COLLABORATION.REMOVED`     | A collaboration has been removed                                                                                    | いいえ   | はい    |
| `COLLABORATION.UPDATED`     | A collaboration has been updated.                                                                                   | いいえ   | はい    |
| `SHARED_LINK.DELETED`       | A shared link was deleted                                                                                           | はい    | はい    |
| `SHARED_LINK.CREATED`       | A shared link was created                                                                                           | はい    | はい    |
| `SHARED_LINK.UPDATED`       | A shared link was updated                                                                                           | はい    | はい    |

<!-- markdownlint-enable line-length -->

<Message type="notice">

When the permissions on an item prevent an action from occurring, no notification is sent for the attempted action.

</Mesage>
