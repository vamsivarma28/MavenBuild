HelloWorld Servlet example with corresponding Dockerfile

Use Maven Build first to create war file in Target folder.

mvn clean package

Artifact will be created in target folder.

docker build -t mavenbuild .

Once this is done u will be see image1 usingg docker images

Use below command to run the container

docker run -d -p 8080:8080 --name mavenbuild mavenbuild
