FROM openjdk:8-jre-alpine
ENV APP_FILE flight-proxy-service-0.5.jar
ENV APP_HOME /usr/apps
EXPOSE 7102
COPY target/$APP_FILE $APP_HOME/
WORKDIR $APP_HOME
ENTRYPOINT ["sh", "-c"]
CMD ["exec java -jar $APP_FILE"]