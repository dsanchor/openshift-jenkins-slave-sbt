FROM registry.access.redhat.com/openshift3/jenkins-slave-maven-rhel7

ENV SBT_VERSION 0.13.15

USER root

# Install sbt
RUN curl -sL "https://dl.bintray.com/sbt/native-packages/sbt/$SBT_VERSION/sbt-$SBT_VERSION.tgz" | gunzip | tar -x -C /usr/local && \
    ln -s /usr/local/sbt/bin/sbt /usr/local/bin && \
    mkdir -p $HOME/.sbt && \
    mkdir -p $HOME/.ivy2

RUN chown -R 1001:0 $HOME && \
    chmod -R g+rw $HOME

USER 1001
