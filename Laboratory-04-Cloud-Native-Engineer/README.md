Mission Overview
  This mission focused on learning the container lifecycle and how to manage Docker containers effectively. It built on previous checkpoints by practicing container deployment, stopping, verifying, and removal.


Objectives
- Understand how to list running containers.
- Practice stopping a container gracefully.
- Verify container states after stopping.
- Remove containers completely from the system.
- Document all Docker lifecycle commands used in Checkpoints 3, 4, and 5.


  Checkpoint 3 – Enter the Docker Playground
- docker --version


  Checkpoint 4 – Deploy Nginx
- docker pull nginx
- docker run -d -p 8080:80 nginx
- curl http://localhost:8080

  
  Checkpoint 5 – The Container Lifecycle
- docker ps
- docker stop <container_id>
- docker ps
- docker rm <container_id>


  Skills Learned
- Running and managing Docker containers.
- Using lifecycle commands (ps, stop, rm) to control container states.
- Deploying applications (Nginx) inside containers.
- Documenting technical processes in Markdown format.

  Challenges Encountered

- Difficulty enabling virtualization on Lenovo laptop BIOS.
- Errors when using placeholder <container_id> instead of actual IDs.
- Needed to use KillerCoda playground as an alternative environment.
- Ensuring proper screenshots (nginx-running.png, container-lifecycle.png) were captured for documentation.
