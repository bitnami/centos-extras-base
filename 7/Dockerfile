FROM centos:7

LABEL maintainer "Bitnami <containers@bitnami.com>"
ENV IMAGE_OS=centos-7

ENV BITNAMI_IMAGE_VERSION=7-r435

COPY rootfs /

# component installation requirements
RUN mkdir --parents /opt/bitnami
RUN yum upgrade -y && \
    install_packages tar gzip curl ca-certificates sudo procps-ng libaio-devel which
