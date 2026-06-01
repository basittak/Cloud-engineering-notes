# Dockerized App - Run Instructions

Build the image:

```
docker build -t dockerized-app:1.0 .
```

Run the container:

```
docker run -p 8080:8080 dockerized-app:1.0
```

Visit http://localhost:8080 to see the app.
