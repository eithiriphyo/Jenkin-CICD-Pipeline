FROM eclipse-temurin:17-jdk

RUN apt-get update && apt-get install -y \
    maven \
    git \
    curl \
    docker.io \
 && rm -rf /var/lib/apt/lists/*

# Create non-root user
RUN useradd -m jenkins
USER jenkins

WORKDIR /home/jenkins
