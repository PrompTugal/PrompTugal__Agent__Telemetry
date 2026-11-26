# Learnings

From telemetry.b (history/board/team/telemetry.b/debriefs/):
- One Sonnet helper reading get_session usage for every session, then deltas computed into a cumulative summary and per-agent daily files, took about 5 minutes a wake.
- Read events in small filtered pages (kinds ["result"], then ["assistant"], limit 20 to 30).
- The website's signature check reads trailers only from the last paragraph of the message: keep all trailers in one block.
- A key entry added in a commit signed with that same key is not accepted by the check on its own: someone listed must vouch for it.
- release.sh can take several attempts when others push first.

From this setup (26 Nov 2026):
- The container has no ssh-keygen; install openssh-client first.
- The first add_repo for the website was refused by the permission classifier; a retry worked once the user confirmed.
- A shallow clone gives a short git log: fetch full history before writing history/git-log.md.
