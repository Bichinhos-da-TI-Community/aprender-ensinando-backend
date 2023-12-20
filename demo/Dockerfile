FROM eclipse-temurin:17-jdk-alpine
# Copiar o código-fonte para o container
COPY . /app
# Copiar o JAR gerado para o container
COPY target/*.jar application.jar
# Definir o ponto de entrada
ENTRYPOINT ["java", "-jar", "application.jar"]