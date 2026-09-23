## Yulio Valdes Cascales

Security-focused developer. I look for authorization and session bugs in open source
projects, then send the fix with tests.

### Recent work

**FileGator**, multi-user file manager (PHP)

- [CVE-2026-94618](https://github.com/filegator/filegator/security/advisories/GHSA-f74m-x83r-c4v4),
  missing authorization in `GET /batchdownload` let any user retrieve another user's
  archive. Reported privately, fixed with regression tests in
  [#597](https://github.com/filegator/filegator/pull/597). Merged.
- [CVE-2026-94619](https://github.com/filegator/filegator/security/advisories/GHSA-44r8-3p76-84mw),
  missing authorization in `POST /upload` allowed cross-user read and deletion of
  temporary files. Fixed in
  [#598](https://github.com/filegator/filegator/pull/598). Merged.
- [GHSA-4r6c-gx7v-584w](https://github.com/filegator/filegator/security/advisories/GHSA-4r6c-gx7v-584w),
  the LDAP auth adapter did not regenerate the session id on login and did not
  revalidate the session user per request. Added both, with tests, in
  [#602](https://github.com/filegator/filegator/pull/602). Merged and shipped in
  7.16.0.
- [#603](https://github.com/filegator/filegator/pull/603) Hardening: hash the upload
  tmpfs namespace so similar usernames cannot collide, and make the session cookie
  Secure over HTTPS. Open.

The LDAP fix shipped downstream in
[HestiaCP 7.16.2](https://github.com/hestiacp/hestiacp/pull/5695).

### Focus

Broken access control, IDOR, session handling, multi-tenant isolation. Mostly PHP and
Python. I write the regression test that proves the bug is gone, not just the patch.

### Open to work

Available for security research, responsible disclosure, and backend or AppSec
collaboration. Reach me through GitHub.
