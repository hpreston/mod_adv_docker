
## Dockerfile: Install Application Requirements 

```
# Application Ports
# Put this after MAINTAINER
EXPOSE 5000

# Install Python requirements
RUN pip install -r /demo_aci_health_dashboard/requirements.txt

# Prep Required Environment Variables
# Target Hank's Lab... can override with another when running
ENV APIC_URL="https://dmz-apic.reqdemo.com" \
    APIC_LOGIN="admin" \
    APIC_PASSWORD="ACIsim12345" \
    APIC_TENANT="SnV"
```

## Build Docker Image 

```bash
docker build -t dockeruser/demo_acidash:latest .
```

