FROM almalinux:9
RUN dnf install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
ADD https://raw.githubusercontent.com/gajuladeepak/terraform-aws-ec2/refs/heads/main/readme.MD /usr/share/nginx/html/index.html
RUN chmod +x /usr/share/nginx/html/index.html
ADD sample-1.tar /tmp/
# what ADD instruction does it extracts and places it /tmp/
CMD ["nginx","-g","daemon off;"]
