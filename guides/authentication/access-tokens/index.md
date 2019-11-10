---
rank: 4
related_endpoints: []
related_guides: []
required_guides: []
related_resources: []
alias_paths: []
cId: authentication
scId: authentication/access-tokens
id: authentication/access-tokens
isIndex: true
---
# Access Tokens

Access Tokens are at the core of every Box API call. They represent an
authenticated user to the Box servers and determine what files and folders an
application has access to.

<CTA to="guide://authentication/select">
Learn about the different ways an app can get authorized

</CTA>

## Application Types & Access Tokens

The following shows how each application type is expected to create an Access
Token.

<!-- markdownlint-disable line-length -->

| Box Application Type               | How to get Access Token              |
| ---------------------------------- | ------------------------------------ |
| Custom App + OAuth 2.0             | [oauth2-with-sdk][oauth2-with-sdk]   |
| Custom App + JWT                   | [jwt-with-sdk][jwt-with-sdk]         |
| Custom App + App Token             | [devtoken][devtoken]                 |
| Enterprise Integration + OAuth 2.0 | [oauth2-with-sdk][oauth2-with-sdk]   |
| Enterprise Integration + JWT       | [jwt-with-sdk][jwt-with-sdk]         |
| Partner Integration + App Token    | Configure token in developer console |
| Custom Skill                       | Access Token in event payload        |

<!-- markdownlint-enable line-length -->

[jwt-with-sdk]: g://authentication/jwt/with-sdk

[oauth2-with-sdk]: g://authentication/oauth2/with-sdk

[devtoken]: g://authentication/access-tokens/developer-tokens
