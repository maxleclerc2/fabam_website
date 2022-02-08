FROM eclipse-temurin:17-jdk-focal

COPY spigot-1.17.1.jar /home/server/server.jar

WORKDIR /home/server/
EXPOSE 25565
ENTRYPOINT ["java", "-Xmx4G", "-Xms4G", "-agentlib:jdwp=transport=dt_socket,server=y,suspend=n,address=*:5005", "-jar", "/home/server/server.jar", "nogui"]

