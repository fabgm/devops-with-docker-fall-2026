# Use the Ubuntu 24.04 base image for the container.
FROM ubuntu:24.04

# Set the working directory inside the container to /usr/src/app.
WORKDIR /usr/src/app

# Copy the script into the working directory.
COPY script.sh .

# Make the script executable so it can be run directly.
RUN chmod +x script.sh

# Install curl so the script can fetch remote resources.
RUN apt update && apt install curl -y

# Run the script when the container starts.
CMD ["./script.sh"]
