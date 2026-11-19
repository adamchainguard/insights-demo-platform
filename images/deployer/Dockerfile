FROM alpine/helm:latest AS helm
WORKDIR /src
COPY . .

FROM amazon/aws-cli:latest
COPY --from=helm /usr/bin/helm /usr/local/bin/helm
