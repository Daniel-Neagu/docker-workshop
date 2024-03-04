FROM node:18
#specifies the base image used for running node.js applications

WORKDIR /exercise/frontend
#sets the working directory to /submission/frontend

COPY package*.json ./
#copies the package.. files ending with .json into the docker image

RUN npm install
#runs the command npm install to install dependencies

COPY . .
#copies everything else from the /backend folder into the docker image

ENV REACT_APP_BACKEND_URL=http://localhost:8001
#sets the environment variable REACT_APP_BACKEND_URL to local host 8001, which is the backend's url

ENV PORT=8000
#sets the environment variable port to 8000

CMD ["npm", "run", "start"]
#specifies the command to be run when the image starts, runs the frontend of the app