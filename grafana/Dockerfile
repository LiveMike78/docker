FROM grafana/grafana
USER root
RUN apk update
RUN apk add npm
RUN apk add git
ADD sample-ocs-grafana-nodejs-main /var/lib/grafana/plugins/sample-ocs-grafana-nodejs-main/
WORKDIR /var/lib/grafana/plugins/sample-ocs-grafana-nodejs-main/
RUN npm ci
RUN npm run build
RUN grafana-cli plugins install gridprotectionalliance-osisoftpi-datasource

