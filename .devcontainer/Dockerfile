# Dev container for the slides/ LaTeX project.
# Full TeX Live so any package (beamer, biblatex-ieee, pgfplots, siunitx,
# algorithm2e, unicode-math, biber, latexmk, Source Sans Pro) is present and
# a new user never has to install anything by hand.
FROM mcr.microsoft.com/devcontainers/base:ubuntu

RUN apt-get update \
    && DEBIAN_FRONTEND=noninteractive apt-get install -y --no-install-recommends \
        texlive-full \
        latexmk \
        biber \
        git \
    && rm -rf /var/lib/apt/lists/*

# The base image already provides the non-root `vscode` user, so files
# created under the mounted workspace keep friendly ownership.
