
## Dockerfile: Install Cobra

```
# Copy ACI Cobra SDK into container
ADD *.egg /tmp/

# Install Cobra and cleanup 
RUN easy_install -Z /tmp/acicobra-2.1_1h-py2.7.egg \
    && easy_install -Z /tmp/acimodel-2.1_1h-py2.7.egg \
    && rm -f /tmp/*.egg
```

## Build Docker Image 

```bash
docker build -t dockeruser/demo_acidash:latest .
```

