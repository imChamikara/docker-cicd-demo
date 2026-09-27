# docker-cicd-demo

A simple Node.js + Express application built for a university Docker + GitHub Actions activity.

## Local Docker Testing

To build and run the Docker container locally:

1. Build the Docker image:
   ```bash
   docker build -t docker-cicd-demo .
   ```

2. Run the Docker container:
   ```bash
   docker run -d -p 3000:3000 --name cicd-demo docker-cicd-demo
   ```

3. Test the endpoints:
   - Root: http://localhost:3000/
   - Healthcheck: http://localhost:3000/health

4. Stop and remove the container:
   ```bash
   docker stop cicd-demo
   docker rm cicd-demo
   ```
