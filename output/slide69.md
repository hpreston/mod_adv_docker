
## Dockerfile: Run Application 

```
# Run Application 
CMD cd /demo_aci_health_dashboard && \
    python run.py
```

## Build Docker Image 

```bash
docker build -t dockeruser/demo_acidash:latest .
```

