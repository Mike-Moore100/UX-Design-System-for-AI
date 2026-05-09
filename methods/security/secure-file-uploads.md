# Secure File Uploads

## What
Secure File Uploads constrain, validate, scan, store, and serve uploaded files safely.

Uploads are untrusted input.

## Why it matters
File uploads can introduce malware, data leaks, storage abuse, and content execution risks.

Secure uploads:
- protect users and infrastructure
- reduce storage abuse
- prevent executable content risks
- improve reliability
- preserve trust

The system must control what is accepted and how it is served.

## When to apply
- avatars
- documents
- imports
- media uploads
- attachments
- CSV uploads
- user-generated content

## How to apply

- restrict allowed file types
- validate file content, not only extension
- limit file size and quantity
- store files outside executable paths
- scan or process risky uploads
- serve files with safe headers

Upload UX should explain limits before failure.

## Implementation rules

- file type allowlist is required
- file size limits must be enforced server-side
- uploaded files must not execute as code
- filenames must be sanitised
- private files need access checks
- error messages must explain allowed formats

## Example

Bad:
- any file type accepted
- file stored in public executable directory
- private attachment URL has no auth check

Good:
- PDF and image allowlist
- content validation
- private signed URLs
- clear upload limits

## Fail conditions

- dangerous file type is accepted
- extension is trusted alone
- uploaded content can execute
- private file is publicly accessible
- upload errors are vague

## Enforcement rule

If users can upload files, validate, limit, store, and serve them as untrusted content.
