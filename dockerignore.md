### Here’s an example of a Dockerfile for setting up an NGINX container, along with a .dockerignore file.

#### SAMPLE Dockerfile

```
# Start with the official NGINX base image
FROM nginx:alpine

# Set a working directory
WORKDIR /usr/share/nginx/html

# Copy the static website files to the image
COPY ./index.html /usr/share/nginx/html

# Expose the default NGINX port
EXPOSE 80

# Start NGINX
CMD ["nginx", "-g", "daemon off;"]

```

#### Folder Structure

```
project/
├── Dockerfile
├── .dockerignore
├── public-html/
│   ├── index.html
│   ├── styles.css
│   └── script.js
└── logs/
    └── access.log

```


#### docker ignore

```
# Ignore logs
logs/

# Ignore system files
*.swp
*.tmp
.DS_Store

# Ignore environment and sensitive files
.env
config/secrets.json

# Ignore build files
node_modules/
build/
dist/

```
