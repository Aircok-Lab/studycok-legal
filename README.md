# studycok-legal

StudyCok legal pages, served by GitHub Pages at <https://aircok-lab.github.io/studycok-legal/>.
The app links to these paths (`app/lib/constants/legal_links.dart` in the studycok repo) — do not rename folders.

| Path | Page |
|---|---|
| `terms/` | 이용약관 |
| `privacy/` | 개인정보 처리방침 |
| `community/` | 커뮤니티 운영정책 |
| `account-deletion/` | 계정 삭제 안내 (Play 계정 삭제 URL) |
| `support/` | 고객 문의 |
| `business/` | 사업자 정보 |

Plain HTML, no build step (`.nojekyll`). No scripts or cookies.

## Before treating it as the effective version

- Fill every `class="todo"` span (`grep -rn 'class="todo"' .`) — `[미정]` = value not given yet, `[확인 필요]` = operator must confirm.
- Remove the `<div class="draft">` banner on each page.
- Facts about collected data come from `app/docs/legal-evidence.md` in the studycok repo. Re-check it when the app or DB changes.
- If the terms or privacy text changes after users have agreed, bump `kTermsVersion` in the app so they consent again.
