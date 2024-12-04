# ref - https://docs.docker.com/reference/dockerfile/
# as mentioned selected lightweight version of node.js
FROM node:18-alpine 

# using ec2 instance for docker as root user
WORKDIR /root/myapp

COPY /root/myapp/package.json ./
# my application code is in myapp directory

RUN npm install

COPY /root/myapp/ ./

EXPOSE 3000

CMD ["npm", "start"]