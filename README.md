# FreeBucket
### This portal help user or community to share/send the gifts back to the people of under privilaged society.

Gifts may be used or new, [**No cash transactions**].

Gifts is a cloud-enabled and desktop application.

## Features
- User can add item(s) to FreeBucket.
- User can put request of item(s) and location with proof.
- User can browse the items category wise.
- User can track the request.
- Track the deliver and verify by proper communication channels.

## Technology Stack
- Python
- Django
- JavaScript
- Postgres


And of course FreeBucket itself is open source with a [public repository]
 on GitHub.

## Installation

FreeBucket requires [Python](https://python.org/) 3 to run.

Install the dependencies and devDependencies.

Install and activate virtual environment for Python.

```sh
cd <porject_dir_path>
pip install -r requirements.txt

```

For production environments...

```sh
<TODO>
```

#### Building for source

For production release:

```sh
gulp build --prod
```

Generating pre-built zip archives for distribution:

```sh
gulp build dist --prod
```

## Docker

FreeBucket is very easy to install and deploy in a Docker container.

By default, the Docker will expose port 8080, so change this within the
Dockerfile if necessary. When ready, simply use the Dockerfile to
build the image.

```sh
cd <project_dir_path>
docker build ......
```

This will create the freebucket image and pull in the necessary dependencies.

Once done, run the Docker image and map the port to whatever you wish on
your host. In this example, we simply map port 8000 of the host to
port 8080 of the Docker (or whatever port was exposed in the Dockerfile):

```sh
docker run -d -p 8000:8080 --restart=always --name=freebucket <youruser>/freebucket:${package.json.version}
```

Verify the deployment by navigating to your server address in
your preferred browser.

```sh
127.0.0.1:8000
```
