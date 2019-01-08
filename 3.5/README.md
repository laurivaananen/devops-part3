Size before changes 1.14GB
Size after changes 19.1MB

Build the image inside the hackernews directory:

`docker build . -t hackernews`

run the image with

`docker run -d -p 5000:80 hackernews`

go to http://localhost:5000 to see the app running
