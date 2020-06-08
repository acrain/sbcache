FROM openjdk:8-alpine
ARG UNPACKED_DIR=target/unpacked
COPY ${UNPACKED_DIR}/BOOT-INF/lib /app/lib
COPY ${UNPACKED_DIR}/META-INF /app/META-INF
COPY ${UNPACKED_DIR}/BOOT-INF/classes /app
ENTRYPOINT ["java", "org.springframework.boot.loader.JarLauncher"]
