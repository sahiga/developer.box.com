---
rank: 150
cId: trash
scId: null
id: trash
isIndex: true
---
# Trash

Before items are deleted they might end up in a user's trash. The trash can be managed by a user through any of the Box apps, and by an application via the API.

## Two-stage Deletion Process

Box uses a two-stage process to remove or **trash** [files][files], [folders][folders], and [web links][web links] before permanently deleting them.

By default, items can be restored after they are **trashed** within a 30 day time frame before they are **purged**. The purge window can be modified by an enterprise administrator.

More details can be found in the Box community article on [Managing Trash][Managing Trash]

[files]: https://box.dev/en/reference/resources/file/

[folders]: https://box.dev/en/reference/resources/folder/

[web links]: https://box.dev/en/reference/resources/web-link/

[Managing Trash]: https://community.box.com/t5/Managing-Files-and-Folders/Manage-Trash/ta-p/19212
