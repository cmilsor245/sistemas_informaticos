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

  <p{
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