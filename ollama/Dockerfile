FROM ubuntu:20.04

# Install dependencies
RUN apt-get update && apt-get install -y \
    python3 python3-pip curl

# Copy configuration and script files
COPY config/ollama_config.yaml /app/config/ollama_config.yaml
COPY scripts/ollama_start.sh /app/scripts/ollama_start.sh
RUN chmod +x /app/scripts/ollama_start.sh

# Set entry point
ENTRYPOINT ["/app/scripts/ollama_start.sh"]
