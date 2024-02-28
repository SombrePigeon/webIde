FROM httpd as base
EXPOSE 80

#DEV-----------
FROM base as dev
ENV VIRTUAL_HOST="view.webide.alexismartial.fr.localhost,view.webide.sombrepigeon.fr.localhost"
ENV LETSENCRYPT_HOST="view.webide.alexismartial.fr.localhost,view.webide.sombrepigeon.fr.localhost"

#PROD----------
FROM base as prod
ENV VIRTUAL_HOST="view.webide.alexismartial.fr,view.webide.sombrepigeon.fr"
ENV LETSENCRYPT_HOST="view.webide.alexismartial.fr,view.webide.sombrepigeon.fr"
