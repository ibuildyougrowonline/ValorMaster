FROM python:3.9-slim
WORKDIR /app
# Copy agent code and prompts
COPY agent/ ./agent/
COPY prompts/ ./prompts/
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
# Default command to register/deploy the agent
ENTRYPOINT ["python", "agent/deploy_agent.py"]
