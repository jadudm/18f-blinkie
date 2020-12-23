# Documentation

This folder contains the documentation for the 18F blinkie. 

The site was initialized with:

```
docker run -v $(pwd):/site bretfisher/jekyll new --force .
```

And, to view edits:

```
docker-compose up
```

Because my local environment seems broken, I had to find the container's IP address:

```
docker container inspect docs_jekyll_1
```

and use a non-standard address. In theory, the docs should be available at `http://localhost:4000`.