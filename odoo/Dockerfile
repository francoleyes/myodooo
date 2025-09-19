ARG ODOO_VERSION
FROM ghcr.io/tecnativa/doodba:${ODOO_VERSION}-onbuild

USER root

# Prepare pyafipws cache directory with correct permissions
RUN mkdir -p /usr/local/lib/python3.10/site-packages/pyafipws/cache \
    && chown -R odoo:odoo /usr/local/lib/python3.10/site-packages/pyafipws/cache

USER odoo
