FROM node

# Now we have to set this directory as our working directory: 
WORKDIR /usr/src/app

# Copy the file package.json to the working directory with the following command:
COPY app /usr/src/app/
COPY package*.json ./
 
# After this we have to run npm install so that we can set up our node environment:
RUN npm install

 
# The app that I am running uses the port 3000, we will be using EXPOSE instruction so that it can be mapped by the docker daemon: 
EXPOSE 3000
 
# And then the final command to start our project with npm start:
CMD ["npm","start"]
