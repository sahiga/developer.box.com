---
rank: 10
alias_paths:
  - /docs/usage-patterns
  - /docs/quickstart-guides
  - /docs/getting-started-box-integration
  - /docs/get-started-with-the-box-api
  - /docs/app-management
  - /docs/configuring-box-platform
cId: applications
scId: null
id: applications
isIndex: true
---
# Applications

Box Platform supports two distinctly different application types. The type of
service you are trying to create determine the type of Box App you will want to configure.

## Overview

The following is quick overview of the different Box Application types.

<ImageFrame>

![Application Types](./images/app-types.png)

</ImageFrame>

<!-- markdownlint-disable line-length -->

| App Type                       | Auth Method             | Features & Limitations                             |
| ------------------------------ | ----------------------- | -------------------------------------------------- |
| [custom-apps][custom-apps]     | [oauth2][oauth2]        | Web App Integrations, App Gallery, Webhooks        |
| [custom-apps][custom-apps]     | [jwt][jwt]              | Webhook                                            |
| [custom-apps][custom-apps]     | [apptoken][apptoken]    | Web App Integrations, Webhooks, Limited API access |
| [custom-skills][custom-skills] | No authorization needed | Limited API access                                 |

<!-- markdownlint-enable line-length -->

<CTA to="guide://applications/select">
Learn how to select an application type

</CTA>

## Additional App Types

A few addition App Types exist for legacy purposes. Please use the alternatives
as specified below.

<!-- markdownlint-disable line-length -->

| App Type               | Auth Method          | Description                                                    |
| ---------------------- | -------------------- | -------------------------------------------------------------- |
| Enterprise Integration | [oauth2][oauth2]     | Equal to a Custom App configured with OAuth 2.0 authentication |
| Enterprise Integration | [jwt][jwt]           | Equal to a Custom App configured with JWT authentication       |
| Partner Integration    | [apptoken][apptoken] | Equal to a Custom App configured with App Token authentication |

<!-- markdownlint-enable line-length -->

[oauth2]: guide://authentication/oauth2

[jwt]: guide://authentication/jwt

[apptoken]: guide://authentication/app-token

[devtoken]: guide://authentication/access-tokens/developer-tokens

[custom-apps]: g://applications/custom-apps

[custom-skills]: g://applications/custom-skills