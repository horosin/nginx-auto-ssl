# Nginx + Let's encrypt gateway
Web application to store and browse patients' clinical data.

## Deployment

First time (to set up let's encrypt ssl keys):
```
cp gateway/init-letsencrypt.sh . && ./init-letsencrypt.sh && rm init-letsencrypt.sh
```

Every other time:
```
docker-compose -f docker-compose.prod.yml up
```
