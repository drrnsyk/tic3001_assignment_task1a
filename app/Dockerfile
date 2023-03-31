FROM node:19

### BUILDING THE IMAGE ###

WORKDIR /app

# copy files
COPY index.js .
COPY package-lock.json .
COPY package.json .
# copy directories
COPY public public 

# install packages
RUN npm i

### RUNNING THE CONTAINER ###

# what port the application listens to
EXPOSE 8080

# run the program
ENTRYPOINT node index.js