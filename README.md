## Yulio Valdes

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

### Focus

Broken access control, IDOR, session handling, multi-tenant isolation. Mostly PHP and
Python. I write the regression test that proves the bug is gone, not just the patch.

### Open to work

Available for security research, responsible disclosure, and backend or AppSec
collaboration. Reach me through GitHub.
