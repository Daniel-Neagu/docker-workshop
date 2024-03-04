FROM node:18 
#specifies the base image used for running node.js applications

WORKDIR /exercise/backend
#sets the working directory to /submission/backend

COPY package*.json ./
#copies the package.. files ending with .json into the docker image

RUN npm install
#runs the command npm install to install dependencies

COPY . .
#copies everything else from the /backend folder into the docker image

ENV PORT=8001
#sets the port to the port 8001

CMD ["node", "index.js"]
#specifies the command to be run when the image starts, runs the backend