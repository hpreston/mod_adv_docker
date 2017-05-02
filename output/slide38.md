
## Steps

1. Log into quay.io
2. Log into containers.cisco.com 
3. Pull down image from quay.io `docker pull quay.io/hpreston/demo:latest`
4. Docker Login to containers.cisco.com
5. Tag images for containers.cisco.com `docker tag quay.io/hpreston/demo:latest containers.cisco.com/hapresto/demo:latest`
6. Push to containers.cisco.com `docker push containers.cisco.com/hapresto/demo:latest`

