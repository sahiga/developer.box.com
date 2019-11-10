---
rank: 4
related_endpoints:
  - post_webhooks
related_guides:
  - webhooks/manage/triggers
  - webhooks/handle/payload
  - webhooks/manage/delete
related_resources:
  - webhook
required_guides: []
alias_paths: []
cId: webhooks
scId: webhooks/manage
id: webhooks/manage/for-folder
isIndex: false
---
# Create Webhook for Folder

To attach a webhook to an folder, call the [1][1] endpoint with the
type of `folder`, the ID of the folder, a URL to send webhook notifications to, and
a list of triggers that will cause the webhook to activate.

<Samples id="post_webhooks" variant="for_folder">

</Samples>

<Message type="warning">

This API requires the application to have the "Manage
webhooks" scope enabled.

The address for the webhook needs to be a HTTPS URL.

</Message>

## Webhook address

The notification URL specified in the `address` parameter must be a
valid HTTPS URL that you specify when you create a webhook. Every
time one of the triggers is activated, this URL will be called.

The notification URL must use the standard HTTPS port, `443` and should be the
should return an HTTP status in the range of `200` to `299` within 30 seconds
of receiving the webhook payload.

## Webhook triggers

トリガーのリストでは、Webhookをトリガーするイベントを表す文字列を指定します。たとえば、ユーザーがファイルをアップロードしたときにWebhookをトリガーするには、トリガー名として`FILE.UPLOADED`を渡します。

使用可能なトリガーのリストは、[2][2]にあります。

[1]: endpoint://post_webhooks

[2]: guide://webhooks/manage/triggers