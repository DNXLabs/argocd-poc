# Argo CD POC


To build our image, run the following command:
```bash
docker build -t webserver .
# or
one build
```

Now we can run our image in a container but this time we do not have to create a bind mount to include our html.
```bash
docker run -it --rm -p 80:80 --name web webserver
# or
one run
```

Open your browser and navigate to http://localhost:8080 to make sure our html page is being served correctly.