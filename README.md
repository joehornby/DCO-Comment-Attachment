# DCO Comment Attachment

DCO Comment Attachment allows your visitors to attach images, videos, audios, documents and other files with their comments. They will also be able to automatically embed links from Youtube, Facebook, Twitter and other services in the comment text.

With plugin settings you can:
- Select an attachment image size from thumbnails available in your WordPress install.
- Link thumbnail to full-size image.
- Limit the maximum file upload size.
- Make an attachment required.
- Specify whether the attachment will be embedded or displayed as a link.
- Enable/Disable autoembed links (like Youtube, Facebook, Twitter, etc.) in the comment text.
- Attach an attachment to a commented post.
- Restrict attachment file types.
- Decide who will be able to upload attachments: all users or only logged users.

You can also:
- Add, replace or delete an attachment from a comment on Edit Comment screen.
- Delete an attachment on Comments screen.

Attachments are uploaded to the WordPress Media Library and deleted along with the comment (if this is set in the settings).

DCO Comment Attachment is also available on [WordPress.org](https://wordpress.org/plugins/dco-comment-attachment/).

# Version
1.3.1

[![Build Status](https://travis-ci.org/yadenis/DCO-Comment-Attachment.svg?branch=dev)](https://travis-ci.org/yadenis/DCO-Comment-Attachment)

# Changelog
## 1.3.1
- Fixed image embed bug when attachment url has get parameters

## 1.3.0
- Added the feature to link a thumbnail to a full-size image.
- Added the feature for restrict uploading attachments only to logged users.
- Added notification about automatically embedded links, when it's enabled.
- Fixed bug with incorrect display of attachment types that do not support embedding.
- Removed jQuery dependency on the frontend.

## 1.2.1
- Fixed Quick Edit Comment function bug

## 1.2.0
- Added the feature for autoembed links in comment text. You can disable it in Settings -> DCO Comment Attachment.
- Introduced `dco_ca_disable_display_attachment` hook. Now you can display attachment in custom place with `add_filter('dco_ca_disable_display_attachment', '__return_true');` filter and `dco_ca()->display_attachment()` function.

## 1.1.2
- Fixed display of empty allowed types if the website administrator has forbidden the upload of all extensions of this type. (thank you [@nunofrsilva](https://github.com/nunofrsilva))

## 1.1.1
- Added filters for the attachment field customization

## 1.1.0
- Now you can select and deselect Allowed File Types by the type in one click.
- Added `dco_ca_disable_attachment_field` hook for disable the upload attachment field.
- Reduced the effect of mime types filtering. Now it applies only for comment attachment upload.
- Added the feature to attach an attachment to a commented post.

## 1.0.0
- Initial Release