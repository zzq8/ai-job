# 多架构原生支持 (amd64/arm64), 体积小, 官方维护
FROM eclipse-temurin:17-jre-jammy

WORKDIR /app

COPY --chown=root:root ai-job.jar /app/ai-job.jar

EXPOSE 9100 6768

ENTRYPOINT ["java", "-jar", "-XX:+StartAttachListener"]
CMD ["/app/ai-job.jar"]
