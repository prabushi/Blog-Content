FROM wso2/micro-integrator:1.1.0
COPY CompositeApps/*.car /home/wso2carbon/wso2mi/repository/deployment/server/carbonapps/
COPY Libs/*.jar /home/wso2carbon/wso2mi/lib/
COPY Resources/cipher-tool.properties /home/wso2carbon/wso2mi/conf/security
COPY Resources/secret-conf.properties /home/wso2carbon/wso2mi/conf/security
COPY Resources/password-tmp /home/wso2carbon/wso2mi
COPY Resources/secure-vault.properties /home/wso2carbon/wso2mi/registry/config/repository/components/secure-vault/
ENV BE_ENDPOINT "http://localhost:8290/services/Hello"
COPY  --chown=wso2carbon:wso2 CarbonHome/.metadata/metadata_config.properties /home/wso2carbon/wso2mi/.metadata/metadata_config.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/passthru-http.properties /home/wso2carbon/wso2mi/conf/passthru-http.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/user-mgt.xml /home/wso2carbon/wso2mi/conf/user-mgt.xml
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/carbon.properties /home/wso2carbon/wso2mi/conf/carbon.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/jndi.properties /home/wso2carbon/wso2mi/conf/jndi.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/datasources/master-datasources.xml /home/wso2carbon/wso2mi/conf/datasources/master-datasources.xml
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/axis2/axis2_blocking_client.xml /home/wso2carbon/wso2mi/conf/axis2/axis2_blocking_client.xml
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/axis2/axis2.xml /home/wso2carbon/wso2mi/conf/axis2/axis2.xml
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/security/cipher-text.properties /home/wso2carbon/wso2mi/conf/security/cipher-text.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/deployment.toml /home/wso2carbon/wso2mi/conf/deployment.toml
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/synapse.properties /home/wso2carbon/wso2mi/conf/synapse.properties
COPY  --chown=wso2carbon:wso2 CarbonHome/conf/carbon.xml /home/wso2carbon/wso2mi/conf/carbon.xml
RUN mkdir /home/wso2carbon/wso2mi/repository/resources/conf/.metadata
COPY  --chown=wso2carbon:wso2 CarbonHome/.metadata/metadata_config.properties /home/wso2carbon/wso2mi/repository/resources/conf/.metadata