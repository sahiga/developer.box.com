---
rank: 6
related_endpoints:
  - delete_webhooks_id
related_guides:
  - webhooks/manage/for-file
  - webhooks/manage/list-all
required_guides:
  - webhooks/manage/for-file
alias_paths: []
cId: webhooks
scId: webhooks/manage
id: webhooks/manage/delete
isIndex: false
---
# Delete Webhook

Box上のファイルやフォルダからWebhookを削除するには、削除するWebhookのIDをAPIに渡す必要があります。

<Samples id="delete_webhooks_id">

</Samples>

<Message type="notice">

# Webhook ID

To find the ID of the webhook, use the [List all webhooks][1] endpoint.

</Message>

## Additional reasons for deletion

Using the API is not the only way a webhook can be deleted.

The following reasons can cause webhooks to be deleted.

1. Deleting a Box application deletes all webhooks associated with the application.
2. Deleting all access tokens associated with a webhook.
3. If webhooks could not be delivered for a system-determined amount of time then Box automatically removes the webhook.

In all of these cases Box would send a webhook payload with the `WEBHOOK.DELETED` event name to the notification URL. In this case the body of the payload will include the following additional information.

```json
"additional_info": {
  "reason": "auto_cleanup"
}
```

[1]: guide://webhooks/manage/list-all
