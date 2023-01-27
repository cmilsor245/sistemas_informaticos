<style>
  h1{
    border: none;
    margin-bottom: 2px;
    text-align: center;
    font-weight: bold;
  }

  img{
    border: 2px solid black;
  }

  p{
    text-align: justify;
  }>
</style>

<h1>DOCKER - E2</h1>

<hr>

<p><b>1. Download and run version 2.4.54-alpine of the web server to access the Apache server via port 8080.</b></p>

```bash
docker run -d -p 8080:80 httpd:2.4.54-alpine
```

<img src="img/ej1.png">

```bash
docker rename pdantic_mcclintock webapache
```

<img src="img/ej1-2.png">

<p><b>2. Access the "webapache" terminal. Locate the default directory where the welcome file is saved. Create a directory called "backupweb" and make a copy of the default page in this directory.</b></p>

```bash
docker exec -it webapache sh
```

<img src="img/ej2.png">

```bash
cd /usr/local/apache2/htdocs
```

```bash
ls -la
```

<img src="img/ej2-2.png">

```bash
mkdir backupweb
```

```bash
cp index.html backupweb/index_copy.html
```

<img src="img/ej2-3.png">

<p><b>3. Exit the "webapache" docker terminal. Locate a complete static project where you have your html works, styles, etc... Copy all the content of this website in the "webapache" container so that we can view the content of our website on the apache server.</b></p>

```bash
docker cp . webapache:/usr/local/apache2/htdocs
```

<img src="img/ej3.png">

<p><b>4. To see if it works, stop the container and then start it again. Visit in a browser the address "localhost:8080".</b></p>

<img src="img/ej4.png">

<p><b>5. Using the image pulled in exercise 1, create a new image using "Dockerfile" to create a container called "nuevaweb", which will be used as a web page, using port 8081.</b></p>

<p>Content in the "Dockerfile" file:</p>

```bash
from httpd:2.4.54-alpine
copy . /usr/local/apache2/htdocs
expose 8081
```

<img src="img/ej5.png">

<p>Building the image, this time I didn't specify the version:</p>

```bash
docker build -t nuevaweb .
```

<img src="img/ej5-2.png">

```bash
docker images
```

<img src="img/ej5-3.png">

<p>An now creating the container from this image:</p>

```bash
docker run -d --name nuevaweb -p 8081 nuevaweb
```

<img src="img/ej5-4.png">

<p>And now it can be visited from a web browser.</p>

<p><b>6. Modify the web page content. What do you need to do?</b></p>

<p>To modify the web page, you must access the container where said page is hosted and modify the code from there.</p>

<p><b>7. To avoid having to rebuild the container on each page source code change web, use a volume that automatically synchronizes the web directory of our host with container web directory. Use the following statement: "docker run -d -p 80:80 -v host_directory:webapache_container_directory".</b></p>

<p>The command "docker run -d -p 80:80 -v host_directory:webapache_container_directory" will run a container in detached mode (-d) and map port 80 of the host to port 80 of the container (-p 80:80). It also creates a volume (-v host_directory:webapache_container_directory) that synchronizes the host directory host_directory with the container's webapache_container_directory directory. This means that any changes made to the files in host_directory will be reflected in the container's webapache_container_directory directory, and vice versa, eliminating the need to rebuild the container each time there is a change to the web source code.</p>

<p><b>8. Check that the previous step works. To do this, it modifies the content of the web page and test that when updating the changes are published by the server.</b></p>

