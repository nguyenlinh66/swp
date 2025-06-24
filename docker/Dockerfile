FROM tomcat:9.0-jdk11

# Xóa ứng dụng mặc định
RUN rm -rf /usr/local/tomcat/webapps/*

# Copy file WAR đã build, đổi tên thành ROOT.war để deploy vào /
COPY target/SWP_TECH-1.0-SNAPSHOT.war /usr/local/tomcat/webapps/ROOT.war

# Tomcat mặc định chạy port 8080 bên trong container
EXPOSE 8080

# Khởi chạy Tomcat
CMD ["catalina.sh", "run"]
