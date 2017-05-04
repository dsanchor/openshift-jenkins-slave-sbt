FROM openshift/jenkins-slave-maven-rhel7

ENV SBT_VERSION 0.13.15

# Install sbt
RUN curl -sL "https://dl.bintray.com/sbt/native-packages/sbt/$SBT_VERSION/sbt-$SBT_VERSION.tgz" | gunzip | tar -x -C /usr/local && \
    ln -s /usr/local/sbt/bin/sbt /usr/local/bin
