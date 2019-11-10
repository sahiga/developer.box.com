---
alias_paths:
  - /sdks
  - /docs/sdks-and-tools
  - /docs/sdks
  - /docs/box-sdks
  - /docs/mobile-sdks
  - /page/sdks
  - /docs/box-sdk-license
centered: true
id: sdks-and-tools
isIndex: true
---
# SDKs & Tools

The following tools are actively developed and supported by Box. These tools
receive regular product updates, as well as security updates.

## Official SDKs & CLIs

| Platform                 | Maintained? | Parity? |
| ------------------------ | ----------- | ------- |
| [javasdk][javasdk]       | はい          | Full    |
| [dotnetsdk][dotnetsdk]   | はい          | Full    |
| [pythonsdk][pythonsdk]   | はい          | Full    |
| [nodesdk][nodesdk]       | はい          | Full    |
| [cli][cli]               | はい          | Full    |
| [iossdk][iossdk]         | はい          | Partial |
| [androidsdk][androidsdk] | はい          | Partial |

<Message type="notice">

**Maintained:** Fully maintained projects are actively developed by Box. They
receive the latest security updates and new features. For support with these
projects please visit GitHub or [forum][forum].

**API Parity**: Projects with full API parity are actively updated with all
platform functionality as this becomes available on the Box Platform. Projects
with partial API parity lack some functionality while we work on bringing
these projects to full parity.

</Message>

## Official UI Libraries

Extend your application with pre-built UI components to browse, share, and
preview files on Box.

<!-- markdownlint-disable line-length -->

|                                                                   |                                                                             |                                                                                      |
| ----------------------------------------------------------------- | --------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| Browse                                                            | Share                                                                       | Preview                                                                              |
| ![Browse][browseimg]                                              | ![Share][shareimg]                                                          | ![Preview][previewimg]                                                               |
| Navigate and manipulate your files on Box using our pre-built UI. | Share files with our pre-built UI elements for file & folder collaboration. | Review over 120 files types, from PDFs to HD videos, with a rich preview experience. |

| Platform   |                                                                                                                                                                                       |
| ---------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| iOS        | [iosbrowsesdk][iosbrowsesdk], [iossharesdkiossharesdk][iossharesdk], [iospreviewsdkiospreviewsdk][iospreviewsdk]                                                                      |
| Android    | [Browse SDK](https://github.com/box/box-android-browse-sdk), [Share SDK](https://github.com/box/box-android-share-sdk), [Preview SDK](https://github.com/box/box-android-preview-sdk) |
| Javascript | [Box UI Elements](guide://embed/ui-elements/)                                                                                                                                         |

<!-- markdownlint-enable line-length -->

<Message type="notice">

**Maintained:** Fully maintained projects are actively developed by Box. They
receive the latest security updates and new features.  For support with these
projects please visit GitHub or [forum][forum]."

</Message>

## Unofficial & Community Tools

The following tools are developed by Box and maintained by Box and its community
members. These tools do not receive regular product updates or security updates.

<!-- markdownlint-disable line-length -->

| Platform                       | Maintained?                           | Parity  |
| ------------------------------ | ------------------------------------- | ------- |
| [salesforcesdk][salesforcesdk] | Limited, by Box and community members | Partial |
| [rubysdk][rubysdk]             | Limited, by Box and community members | Partial |
| [jssdk][jssdk]                 | Limited, by Box and community members | Partial |
| [chromesdk][chromesdk]         | Limited, by Box and community members | Partial |

<!-- markdownlint-enable line-length -->

<Message type="notice">

**Maintained:** Projects with limited maintenance are updated by Box in
collaboration with the community. They receive irregular security updates. If
you are a Box customer on a premium support plan, please contact customer
services for any urgent feature requests for these tools. For other support
queries with these projects please visit GitHub or [forum][forum].

**API Parity:**  Projects with limited API parity can lack some functionality
as new features are not automatically rolled out to these projects as they
become available for the Box Platform. If you are a Box customer on a premium
support plan, please contact customer services for any urgent feature requests
for these tools.

</Message>

[javasdk]: https://github.com/box/box-java-sdk

[dotnetsdk]: https://github.com/box/box-windows-sdk-v2

[pythonsdk]: https://github.com/box/box-python-sdk

[nodesdk]: https://github.com/box/box-node-sdk

[iossdk]: https://github.com/box/box-ios-sdk

[androidsdk]: https://github.com/box/box-android-sdk

[cli]: https://github.com/box/boxcli

[forum]: https://community.box.com/t5/Platform-and-Development-Forum/bd-p/DeveloperForum

[browseimg]: ./browse.jpg

[shareimg]: ./share.jpg

[previewimg]: ./preview.jpg

[iosbrowsesdk]: https://github.com/box/box-ios-browse-sdk

[iossharesdk]: https://github.com/box/box-ios-share-sdk

[iospreviewsdk]: https://github.com/box/box-ios-preview-sdk

[salesforcesdk]: https://github.com/box/box-salesforce-sdk

[rubysdk]: https://github.com/cburnette/boxr

[jssdk]: https://github.com/allenmichael/box-javascript-sdk

[chromesdk]: https://github.com/box/Chrome-App-SDK
