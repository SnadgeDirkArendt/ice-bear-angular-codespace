FROM baseImage as stage

RUN su node -c "npm install axios"
RUN su node -c "npm install -g @angular/cli"

RUN apt-get update && \
    apt-get -y install --no-install-recommends \
        libgtk2.0-0 \
        libgtk-3-0 \
        libgbm-dev \
        libnotify-dev \
        libgconf-2-4 \
        libnss3 \
        libxss1 \
        libasound2 \
        libxtst6 \
        xauth \
        xvfb
# Cypress
RUN su node -c "npm install -g cypress"