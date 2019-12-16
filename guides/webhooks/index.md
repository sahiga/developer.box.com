---
rank: 190
related_endpoints:
  - get_webhooks
  - get_webhooks_id
  - post_webhooks
  - put_webhooks_id
  - delete_webhooks_id
related_resources:
  - webhook
related_guides: null
required_guides: []
alias_paths:
  - /docs/work-with-webhooks
  - /docs/file-workflow-with-webhooks
  - /docs/webhooks
  - /docs/getting-started-with-webhooks-v2
cId: webhooks
scId: null
id: webhooks
isIndex: true
---
# Webhook

Webhookを使用すると、Box上のファイルやフォルダにイベントトリガーを追加できます。

イベントトリガーは、項目に対して発生したイベントを監視し、イベントが発生すると、指定されたURLにHTTPリクエストを送信してアプリケーションに通知します。

Webhookの動作はAPIを介してきめ細かく制御できるため、アプリケーションでは必要に応じてファイルやフォルダにWebhookを追加し、不要になった時点で削除できます。
