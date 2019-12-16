---
rank: 6
related_endpoints:
  - post_oauth2_revoke
related_resources: []
related_guides: []
required_guides:
  - authentication/access-tokens
alias_paths: []
cId: authentication
scId: authentication/access-tokens
id: authentication/access-tokens/revoke
isIndex: false
---
# Revoke a Token

An Access Token can be revoked at any time by either sending the Access Token or Refresh Token the [`POST
/oauth2/revoke`](endpoint://post-oauth2-revoke) endpoint.

<Samples id="post_oauth2_revoke">

</Samples>

<Message>

# Usage in SDKs

All of the Box SDKs support manually revoking the current Access Token associated with the client. To revoke a specific token, first initialize a new SDK with that token and then call the relevant revoke method.

</Message>
