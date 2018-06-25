FROM nuwanbando/javabase

RUN mkdir wso2 

COPY packs/wso2ei-6.2.0.1528984496940.zip wso2/

RUN cd wso2/ && \
        unzip wso2ei-6.2.0.1528984496940.zip

COPY esb/conf/axis2.xml /wso2/wso2ei-6.2.0/conf/axis2/

CMD ["sh", "/wso2/wso2ei-6.2.0/bin/integrator.sh"]

EXPOSE 9763
EXPOSE 9443
EXPOSE 8280
EXPOSE 8243