```shell
sudo docker build -t yiluxiangbei/apprtc:v1 -f docker/Dockerfile .
sudo docker push yiluxiangbei/apprtc:v1

sudo docker login --username yiluxiangbei
sudo docker logout

sudo docker run --rm -it yiluxiangbei/apprtc:v1
sudo docker run --name apprtc -it -d yiluxiangbei/apprtc:v1

sudo docker exec -it apprtc sh
netstat -tlnp

sudo docker stop apprtc
sudo docker start apprtc
sudo docker rm apprtc

sudo docker run --rm  -p 8080:8080 -p 8089:8089 -p 3478:3478 -p 3478:3478/udp -p 3033:3033  --expose=59000-65000 -e PUBLIC_IP=<server public IP> -t -i piasy/apprtc-server

139.59.6.242
xvido365.com
randomcalling

apt install docker-compose
sudo chown nginx:nginx /cert/cert.pem
sudo chown nginx:nginx /cert/key.pem
cd docker
sudo docker-compose up -d
sudo docker-compose down
sudo docker-compose logs -f

sudo docker-compose stop apprtc-web
sudo docker-compose start apprtc-web

https://xvido365.com/
https://www.xvido365.com/

sudo docker exec -it apprtc-web sh

sudo docker pull piasy/apprtc-server
sudo docker run --rm \
  -p 8080:8080 -p 8089:8089 -p 3478:3478 -p 3478:3478/udp -p 3033:3033 \
  --expose=59000-65000 \
  -e PUBLIC_IP=<server public IP> \
  -v <path to constants.py>:/apprtc_configs \
  -t -i piasy/apprtc-server

sudo docker run --rm \
  -p 8080:8080 -p 8089:8089 -p 3478:3478 -p 3478:3478/udp -p 3033:3033 \
  --expose=59000-65000 \
  -e PUBLIC_IP=139.59.6.242 \
  -v /home/web/apprtc/docker/config:/apprtc_configs \
  -t -i piasy/apprtc-server

/opt/app/bin/collidermain -port=443 -tls=true
```