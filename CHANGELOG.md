# Changelog

## 1.0.0 - 2026-09-28

First release.

- Submits discussions to IndexNow when they are started, get a reply, are edited, renamed, retagged, approved,
  hidden, restored or deleted. Only discussions that guests can see are submitted; a discussion that is being
  hidden or deleted is submitted if it was public until then.
- Serves the key file at `/<key>.txt` and sends its location with every request, so forums in a subdirectory work.
- Settings: the key (generated on install), the endpoint (IndexNow.org, Bing, Yandex, Seznam, Naver, Yep, Internet
  Archive, Amazonbot or any other address), a switch for each kind of change, and the result of the last submission.
- `php flarum indexnow:submit --all` submits every public discussion; `php flarum indexnow:submit <url>...` submits
  the given addresses.
- English and Russian translations.
