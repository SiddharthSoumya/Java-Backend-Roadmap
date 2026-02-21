Quick reference:

# Linux Commands Checklist for Java Spring Boot Backend Engineer

## 🔧 System Monitoring
- `top` → Monitor CPU/memory usage
- `htop` → Interactive process viewer
- `ps aux | grep <process>` → Find running processes
- `df -h` → Check disk usage
- `du -sh <dir>` → Check directory size
- `free -m` → Check memory usage
- `uptime` → Show system load and uptime

## 📜 Logs & Debugging
- `tail -f /var/log/syslog` → Follow system logs
- `tail -f logs/spring.log` → Follow Spring Boot app logs
- `grep "ERROR" logs/spring.log` → Search for errors
- `less logs/spring.log` → Scroll through logs
- `journalctl -u <service>` → View logs for a systemd service

## 🌐 Networking
- `ping <host>` → Test connectivity
- `curl http://localhost:8080/actuator/health` → Check Spring Boot health endpoint
- `ss -tuln` → List listening ports
- `netstat -tuln` → Alternative to check ports
- `telnet <host> <port>` → Test port connectivity
- `dig <domain>` → DNS lookup

## ⚙️ Process & Service Management
- `systemctl start <service>` → Start service
- `systemctl stop <service>` → Stop service
- `systemctl restart <service>` → Restart service
- `systemctl status <service>` → Check service status
- `kill -9 <pid>` → Force kill process
- `pkill -f <process-name>` → Kill process by name

## 📦 Java & Spring Boot
- `java -version` → Check Java version
- `mvn clean install` → Build project with Maven
- `./mvnw spring-boot:run` → Run Spring Boot app
- `java -jar target/app.jar` → Run packaged JAR
- `export JAVA_HOME=/path/to/java` → Set Java home
- `echo $JAVA_HOME` → Verify Java home

## 🗄️ File & Directory Operations
- `ls -lah` → List files with details
- `cd <dir>` → Change directory
- `pwd` → Print working directory
- `cp <src> <dest>` → Copy files
- `mv <src> <dest>` → Move/rename files
- `rm -rf <dir>` → Remove directory
- `find . -name "*.log"` → Find log files

## 🔐 Permissions & Ownership
- `chmod 755 <file>` → Change file permissions
- `chown user:group <file>` → Change file ownership
- `whoami` → Show current user
- `groups` → Show user groups

## 🐳 Docker (if used for deployment)
- `docker ps` → List running containers
- `docker logs <container>` → View container logs
- `docker exec -it <container> bash` → Access container shell
- `docker-compose up -d` → Start services
- `docker-compose down` → Stop services

---

✅ This checklist covers **system monitoring, debugging, networking, Java/Spring Boot basics, file operations, permissions, and Docker** — the essentials for a backend engineer working with Spring Boot on Linux.
