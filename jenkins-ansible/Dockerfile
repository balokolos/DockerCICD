FROM jenkins/jenkins

USER root

RUN apt-get update && \
    apt-get install -y python3-pip python3-venv && \
    python3 -m venv /opt/venv && \
    /opt/venv/bin/pip install --upgrade pip && \
    /opt/venv/bin/pip install ansible

ENV PATH="/opt/venv/bin:$PATH"

USER jenkins
