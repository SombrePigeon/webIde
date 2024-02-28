FROM lscr.io/linuxserver/code-server as base
EXPOSE 8443

#DEV-----------
FROM base as dev
ENV VIRTUAL_HOST="code.webide.alexismartial.fr.localhost,code.webide.sombrepigeon.fr.localhost"
ENV LETSENCRYPT_HOST="code.webide.alexismartial.fr.localhost,code.webide.sombrepigeon.fr.localhost"

#PROD----------
FROM base as prod
ENV VIRTUAL_HOST="code.webide.alexismartial.fr,code.webide.sombrepigeon.fr"
ENV LETSENCRYPT_HOST="code.webide.alexismartial.fr,code.webide.sombrepigeon.fr"
