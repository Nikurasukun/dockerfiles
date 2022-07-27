FROM ghcr.io/nikurasukun/almalinux_rpmfusion:latest
MAINTAINER nikurasukun
RUN dnf install nodejs ffmpeg git -y
RUN git clone --depth 1 --branch 0.4.0 https://codeberg.org/teddit/teddit.git
WORKDIR teddit
RUN npm install --no-optional
RUN cp config.js.template config.js
CMD npm start
