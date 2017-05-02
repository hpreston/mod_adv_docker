
## Dockerfile: Get Application Code

```
# Get Application Code
RUN git clone https://github.com/hpreston/demo_aci_health_dashboard /demo_aci_health_dashboard
```

## Build Docker Image 

```bash
docker build -t dockeruser/demo_acidash:latest .
```

