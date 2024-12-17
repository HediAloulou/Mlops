# Use the official Jenkins LTS (Long-Term Support) image from Docker Hub
FROM jenkins/jenkins:lts

# Set environment variables (optional)
ENV JENKINS_USER=admin
ENV JENKINS_PASS=admin

# Install Docker (optional, for Jenkins to run Docker commands)
USER root
RUN apt-get update && apt-get install -y docker.io

# Expose necessary Jenkins ports
EXPOSE 8080 50000

# Set the entry point (already set in the base image)
ENTRYPOINT ["jenkins-lts"]

# Add your own scripts or configuration files if needed (optional)
# COPY your-script.sh /usr/local/bin/your-script.sh