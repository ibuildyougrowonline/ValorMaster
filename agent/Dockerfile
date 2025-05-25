FROM python:3.9-slim
WORKDIR /app
COPY requirements.txt ./
RUN pip install --no-cache-dir -r requirements.txt
COPY agent/ agent/
COPY prompts/ prompts/
ENTRYPOINT ["python", "agent/deploy_agent.py"]
