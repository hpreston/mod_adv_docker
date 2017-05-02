
## Dockerfile: Create Base

```
FROM python:2.7-alpine
MAINTAINER Your Name <your@email.address>

# Install basic utilities
RUN apk add -U \
        ca-certificates \
        git \
  && rm -rf /var/cache/apk/* \
  && pip install --no-cache-dir \
          setuptools \
          wheel
```

## Build Docker Image 

```bash
docker build -t dockeruser/demo_acidash:latest .
```

