FROM ghcr.io/camptocamp/odoo-project:14.0-latest-batteries
MAINTAINER The Open Source Company

# Project's specifics packages
RUN DEBIAN_FRONTEND=noninteractive && \
    apt-get update && \
    apt-get install -y python-shapely git vim && \
    apt-get clean

COPY ./requirements.txt /odoo/
RUN cd /odoo && pip install -r requirements.txt


