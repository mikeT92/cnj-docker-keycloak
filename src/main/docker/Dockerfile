FROM jboss/keycloak:${keycloak.version}

ARG ARG_KEYCLOAK_IMPORT="/tmp/realm-export.json"

LABEL maintainer="michael.theis@hm.edu" \
        ${project.groupId}.${project.artifactId}.project="HMFWPCNJ" \
        ${project.groupId}.${project.artifactId}.version="${project.version}" \
        ${project.groupId}.${project.artifactId}.description="${project.description}" \
        ${project.groupId}.${project.artifactId}.keycloak.version="${keycloak.version}"

COPY cloudtrain-realm-export.json ${ARG_KEYCLOAK_IMPORT}

ENV KEYCLOAK_IMPORT=${ARG_KEYCLOAK_IMPORT}