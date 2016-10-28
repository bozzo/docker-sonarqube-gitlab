FROM sonarqube:lts-alpine

MAINTAINER bozzo

ENV GITLAB_PLUGIN_VERSION 1.7.0
ENV GITLAB_AUTH_PLUGIN_VERSION 1.0.0

RUN curl -o ${SONARQUBE_HOME}/lib/bundled-plugins/sonar-gitlab-plugin-${GITLAB_PLUGIN_VERSION}.jar -sSL "http://nexus.talanlabs.com/content/groups/public_release/com/synaptix/sonar-gitlab-plugin/${GITLAB_PLUGIN_VERSION}/sonar-gitlab-plugin-${GITLAB_PLUGIN_VERSION}.jar" && \
	curl -o ${SONARQUBE_HOME}/lib/bundled-plugins/sonar-auth-gitlab-plugin-${GITLAB_AUTH_PLUGIN_VERSION}.jar -sSL "http://nexus.talanlabs.com/content/groups/public_release/com/synaptix/sonar-auth-gitlab-plugin/${GITLAB_AUTH_PLUGIN_VERSION}/sonar-auth-gitlab-plugin-${GITLAB_AUTH_PLUGIN_VERSION}.jar"
