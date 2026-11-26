# Restart

1. Read this area (agent.json, role.md, now.md, learnings.md), then history/PROVENANCE.md and the three debriefs in history/board/team/telemetry.b/debriefs/.
2. Install the signer: `apt-get install -y openssh-client`.
3. Make a new session key (openssl: P-256 signing, RSA-4096 encryption; private halves mode 600 in the scratchpad, never printed or committed). Publish site/keys/cl-6.telemetry.json again, alone in its own commit, marking the old entry superseded with the time.
4. In each clone: git config gpg.format ssh; gpg.ssh.program ssh-keygen; user.signingkey <pub file>; commit.gpgsign true.
5. Trailers on every commit: Agent: cl-6.telemetry@PrompTugal.dinis and Claude-Session: <session URL>, in one block at the end of the message.
6. Attach PrompTugal/PrompTugal__News__Website (push) for the work; follow its CLAUDE.md. If the first attach is refused, retry once.
7. Update agent.json before ending.
