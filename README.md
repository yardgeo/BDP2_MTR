# BDP2 “Mid-term” Review Project

## Project Description
The project consists of 4 modules:
1. .github/workflows - action configuration. Build & push docker image to dockerhub.
2. data-analysis-docker - configuration jupiter notebook docker image with pre-installed requirements.
3. data-analysis-work - directory for saving .ipybn files/projects.
4. nginx - for configuring proxy-server and https requests.

## Pre-requirements 
For the https connection configuration, certbot was used to obtain certificates from the let's encrypt resource. Command :

```
sudo apt install certbot
certbot certonly --manual -d *.exgratia.ru -d exgratia.ru --agree-tos --no-bootstrap --manual-public-ip-logging-ok --preferred-challenges dns-01 --server https://acme-v02.api.letsencrypt.org/directory
```

The exgratia.ru domain was bought by Georgii Iardukhin for personal purposes.

## To launch
```
git clone https://github.com/yardgeo/BDP2_MTR.git
docker-compose up -d --build
```

## Notes
Project is not available for public usage.

To get access via bdp.exgratia.ru please contact Georgii Iardukhin
georgii.iardukhin@studio.unibo.it 