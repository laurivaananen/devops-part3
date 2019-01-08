Build the container with

`docker build . -t yle-dl`

Download podcast to your own computer with

`docker run -v $(pwd):/app yle-dl https://areena.yle.fi/1-50026325`
