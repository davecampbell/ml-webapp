how to run:

build the image:
$ build -t ml-webapp .

run the container and the app:
- bind a container dir to the app directory
- expose the port 8501 to the host
- run the app from the 'local' directory that has been bound to a container app

$ docker run --rm -p 8501:8501 -v /Users/dcampbell/Documents/projects/ml-webapp/app:/app ml-webapp streamlit run /app/iris-ml-app.py

open browser on host to http://127.0.0.1:8501

