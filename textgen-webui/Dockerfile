FROM ubuntu:20.04

# Install dependencies
RUN apt-get update && apt-get install -y \
    python3 python3-pip curl

# Copy configuration and script files
COPY config/textgen_config.json /app/config/textgen_config.json
COPY scripts/textgen_start.sh /app/scripts/textgen_start.sh
RUN chmod +x /app/scripts/textgen_start.sh

# Set entry point
ENTRYPOINT ["/app/scripts/textgen_start.sh"]
