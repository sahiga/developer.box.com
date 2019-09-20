---
rank: 1
related_endpoints: []
related_guides: []
required_guides: []
alias_paths:
  - /docs/work-with-webhooks
  - /docs/file-workflow-with-webhooks
id: automation-and-events/webhooks
cId: automation-and-events
scId: automation-and-events/webhooks
isIndex: true
---
# Webhook

Webhookを使用すると、Box上のファイルやフォルダにイベントトリガーを追加できます。

イベントトリガーは、項目に対して発生したイベントを監視し、イベントが発生すると、指定されたURLにHTTPリクエストを送信してアプリケーションに通知します。

Webhookの動作はAPIを介してきめ細かく制御できるため、アプリケーションでは必要に応じてファイルやフォルダにWebhookを追加し、不要になった時点で削除できます。

## スコープと権限

アプリケーションの開発者コンソールの構成タブで、\[webhookを管理]アプリケーションスコープが有効になっていることを確認してください。これが有効になっていない場合、API呼び出しを実行しようとすると`403`エラーが返されます。
