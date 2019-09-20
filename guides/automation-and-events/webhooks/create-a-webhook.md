---
rank: 2
related_endpoints:
  - post_webhooks
related_guides:
  - automation-and-events/webhooks/list-of-event-types
  - automation-and-events/webhooks/parse-a-webhook
  - automation-and-events/webhooks/delete-a-webhook
required_guides: []
alias_paths: []
id: automation-and-events/webhooks/create-a-webhook
cId: automation-and-events
scId: automation-and-events/webhooks
isIndex: false
---
# Webhookの作成

項目にWebhookを追加するには、[1][1]項目の種類とID、Webhook通知の送信先URL、およびWebhookをアクティブにするトリガーのリストを指定してエンドポイントを呼び出します。

<Samples id="post_webhooks">

</Samples>

現在サポートされている項目の種類は、`file`と`folder`です。

通知URLは、Webhookの作成時に指定した有効なHTTPS URLである必要があります。このURLは、いずれかのトリガーがアクティブになるたびに呼び出されます。

トリガーのリストでは、Webhookをトリガーするイベントを表す文字列を指定します。たとえば、ユーザーがファイルをアップロードしたときにWebhookをトリガーするには、トリガー名として`FILE.UPLOADED`を渡します。

使用可能なトリガーのリストは、[2][2]にあります。

[1]: ../../../reference/automation-and-events/#post-webhooks

[2]: ../../../reference/automation-and-events/#post_webhooks-triggers
