# pf-uptime-net

Out-of-band uptime monitor for `pianofantasy.com` and `app.pianofantasy.com`.

This repository is **public on purpose**: public repositories get free, unlimited
standard GitHub-hosted runner minutes, which is what makes continuous
minute-resolution monitoring affordable. It therefore contains **no secrets** —
only two already-public hostnames and a `curl` probe.

The alarm channel is GitHub's built-in workflow-failure email to the account
owner. Nothing here can reach, or be reached from, the monitored systems.

See the extensive header comments in
`.github/workflows/pf-uptime-net.yml` for the full design rationale, including
why it does not rely on GitHub's `schedule` event and why the platform probe must
stay database-free.

Owner: Sage.
