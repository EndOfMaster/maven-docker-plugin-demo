FROM java:8-jre-alpine
COPY maven-docker-plugin-test-1.0.jar /app.war
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
EXPOSE 80
ENTRYPOINT ["java","-jar","/app.war"]