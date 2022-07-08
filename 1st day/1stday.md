container: giống cái repo bên github

lệnh docker pull nginx 

lệnh docker run -it -p 8080:80 nginx

docker ps

docker iamges 

docker ps -a 

docker ps -a

do

docker run -d -p 8080:80 nginx
docker run -d -p 8080:80 --name mynginx nginx 

docker start 
docker stop


docker exec -it mynginx bash

docker run -d -p 8080:80 --name mynginx nginx -v html:usr/share/nginx/html
lấy toàn bộ html đập vào nội dụng html kia 


docker logs 

docker run -d -p 8080:80 --name mynginx -v "path":"path2" 




dockerfile  file hưỡng dân tạo ra 1 cái image mới 
FROM nginx
COPY html /usr/share/nginx/html

docker build -t my_nginx_vietnam .

docker run -d -p 8080:80 --name mynginx-vietnam my_nginx_vietnam

docker ps -a


docker push username/name_iamage:tags
