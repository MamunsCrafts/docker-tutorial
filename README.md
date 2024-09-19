# docker-tutorial



## Instalation Guide 
[How To Install and Use Docker on Ubuntu 22.04](https://www.digitalocean.com/community/tutorials/how-to-install-and-use-docker-on-ubuntu-22-04)



## OS name check
```
uname
```
### Docker Interect with ubuntu or node
```
docker run -it node
```

```
docker run -it ubunto
```

### Check How many docker images?
```
docker images
```


### Docker Command 
###Name :  Dockerfile

```
# Use the official Node.js image
FROM node:18

# Set the working directory inside the container
WORKDIR /usr/src/app

# Copy package.json and package-lock.json
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy the rest of the application code
COPY . .

# Expose the application port
EXPOSE 3000

# Start the application
CMD ["npm", "start"]


```
### Docker image build If you stay in current directory

```
docker build -t aws-app .

```


### Run docker images 
#### 3000 port mapping for running  localhost 
```
docker run -p 3000:3000 aws-app

```