```shell
sudo docker build -t yiluxiangbei/apprtc:v1 -f docker/Dockerfile .
sudo docker push yiluxiangbei/apprtc:v1

sudo docker login --username yiluxiangbei
sudo docker logout

sudo docker run --rm  -p 8080:8080 -p 8089:8089 -p 3478:3478 -p 3478:3478/udp -p 3033:3033  --expose=59000-65000 -e PUBLIC_IP=<server public IP> -t -i piasy/apprtc-server
```