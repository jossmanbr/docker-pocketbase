# PocketBase Dockerfile

This is the recommended `Dockerfile` from PocketBase's website.

## Usage

```sh
# create image
sudo docker build -t pocketbase .

# create container (run on default port 8090 on host)
sudo docker run -d --name=pocketbase-0 -p 8090:8080 --restart unless-stopped pocketbase

# stop container
sudo docker stop pocketbase-0

# start container
sudo docker start pocketbase-0
```

## Admin Portal

With PocketBase running in the Docker container, the admin portal can be accessed the same as if locally installed on the host, through http://localhost:8090/\_/
