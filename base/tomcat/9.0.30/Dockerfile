FROM tomcat:9-jdk11

LABEL maintainer="phithon <root@leavesongs.com>"

RUN set -ex \
    && sed -i 's/securerandom\.source=file:\/dev\/random/securerandom.source=file:\/dev\/.\/urandom/g' $JAVA_HOME/jre/lib/security/java.security \
    && rmdir webapps \
    && mv webapps.dist webapps