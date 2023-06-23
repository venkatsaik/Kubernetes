# download base image 
FROM node:alpine    

# move to working dir /APP
WORKDIR /app

# expose the port 3000 as the node-js app is listening at port 3000 
EXPOSE 3000

# copy the package files from the current directory to /app()
COPY package.json package-lock.json ./

# Run npm install to install node modules
RUN npm install

# copy rest of the files
COPY . ./

# now run nom start to start the application
CMD [ "npm", "start" ]

