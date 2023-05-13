# syntax=docker/dockerfile:1.3-labs

FROM ghcr.io/void-linux/void-linux:20230204rc01-thin-x86_64
RUN <<EOF
xbps-install -Syu
xbps-install -Syu
xbps-install -Syu bash less ncurses-base shadow curl python3 tar gzip findutils  util-linux   gleam erlang nodejs git
chsh -s /bin/bash root
rm var/cache/xbps/*
EOF

ENV HOME=/root

CMD [ "sleep", "infinity" ]
