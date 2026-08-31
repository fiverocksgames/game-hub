# Share validation evidence

Date: 2026-08-31

## Scope

FiveRocks GameHub generic share behavior.

## Observed target

- OS: Android (Samsung device screenshot)
- Receiving app: KakaoTalk
- Browser/share path: mobile Web Share / clipboard share path
- Previous payload: title + text + URL
- Actual result: the message contained descriptive text plus the URL, but KakaoTalk did not render the GameHub Open Graph preview.
- Control observation: sharing the FiveRocksGames homepage as a URL produced its OG preview card in the same receiving app.

## Project exception

Per `fiverocksgames/devops-standards/ux/web/share/SHARING_POLICY.md` section 13, GameHub temporarily deviates from the canonical text + link generic profile for this target-platform compatibility issue.

Current generic share payload:

- Web Share API: URL only
- Clipboard fallback: URL only
- Shared URL: `https://fiverocksgames.github.io/game-hub/?share=20260831-kakao-preview-1`

The static query parameter intentionally creates a new receiving-platform cache key while serving the same GitHub Pages document. It contains no user, auth, analytics, or private data.

## Revalidation

Re-test Android + KakaoTalk after deployment. If URL-only sharing reliably renders the OG preview, keep the exception until a later platform re-test demonstrates that text + URL preserves the preview.
