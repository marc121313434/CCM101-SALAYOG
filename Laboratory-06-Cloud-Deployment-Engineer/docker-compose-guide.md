What does the services: block do?
- The services: block defines the containers that make up your application stack. Each service (e.g., database, app) specifies the image to use, environment variables, ports, and other configurations. Docker Compose uses this block to orchestrate multiple containers together as one deployment.
How did the Nextcloud app container know how to find the database container?
- The Nextcloud app container connects to the database using the MYSQL_HOST=database environment variable. Docker Compose automatically creates a network where services can communicate by their names. In this case, the app resolves database as the hostname of the MariaDB container.
Difference between docker run and docker-compose up -d
- docker run starts a single container with specific options (image, ports, environment variables).

- docker-compose up -d launches an entire stack of containers defined in the YAML file, automatically handling networking, dependencies, and scaling. It’s more efficient for multi-container applications since you manage everything from one configuration file.
Mission Overview
- This mission focused on deploying a multi-tier cloud application using Docker Compose. The goal was to set up Nextcloud with a MariaDB backend, document the architecture, and practice container orchestration in a cloud-native environment.
Objectives
- Define and document a two-tier architecture (Web/Application + Database).
- Write infrastructure code using Docker Compose.
- Deploy Nextcloud and MariaDB in separate containers.
- Access the Nextcloud web interface via port 8080.
- Shut down the deployment gracefully.
  
Commands Executed

# Create project directory
mkdir nextcloud-deployment
cd nextcloud-deployment

# Create Compose file
nano docker-compose.yml

# Deploy containers
docker-compose up -d

# Verify running containers
docker-compose ps

# Access Nextcloud via port 8080

# Shut down deployment


docker-compose down
Skills Learned
- Writing and understanding Docker Compose YAML files.
- Deploying and managing multi-container applications.
- Configuring environment variables for container communication.
- Accessing containerized applications through exposed ports.
- Documenting technical processes in Markdown for client-ready deliverables.
