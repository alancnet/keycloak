FROM jboss/keycloak:1.2.0.Beta1

RUN echo 'JAVA_OPTS="$JAVA_OPTS -Dkeycloak.import=/opt/jboss/keycloak/testrealm.json"' >> /opt/jboss/keycloak/bin/standalone.conf
ADD files/testrealm.json /opt/jboss/keycloak/testrealm.json
ADD files/wars/ /opt/jboss/keycloak/standalone/deployments/
