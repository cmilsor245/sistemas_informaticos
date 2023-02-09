<style>
  h1{
    border: none;
    margin-bottom: 0px;
    text-align: center;
    font-weight: bold;
  }

  p{
    text-align: justify;
  }

  img{
    border: 2px solid black;
  }
</style>

<h1>AWS - EXERCISE 1</h1>

<hr>

<p><b>1. Create a new EC2 instance. Name it "UbuntuDockerAWS".</b></p>

<img src="img/1.1.png">

<img src="img/1.2.png">

<img src="img/1.3.png">

<img src="img/1.4.png">

<img src="img/1.5.png">

<p><b>2. Use this EC2 instance to do the following tasks:</b></p>

<p><b>a. Access to this instance using SSH client. Create a new profile.</b></p>

<p>First, I create a new session and configure it to use my new instance's host and the default user "ubuntu". Also, I downloaded the "PPK" file, since I configured it to use a vockey.</p>

<img src="img/2.1.png">

<img src="img/2.2.png">

<p><b>b. Update the Ubuntu packages.</b></p>

```bash
sudo apt update -y && sudo apt upgrade -y && sudo apt auto-remove -y
```

<img src="img/2.3.png">

<p><b>c. Install Docker in this server.</b></p>

```bash
sudo apt install docker.io
```

<img src="img/2.4.png">

<p><b>d. Use WinSCP to transfer the content of a static web page to home directory.</b></p>

<p></p>