# Python Hello World

Run a Python application in a virtual machine

```
git clone https://github.com/fabio-particles/python-hello-world.git
cd python-hello-world
```

To run the Hello World app on your virtual machine:

If you don't have virtualenv, install it using pip.

```
sudo pip install virtualenv
```

Create an isolated Python environment, and install dependencies:

```
virtualenv env
source env/bin/activate
pip install -r requirements.txt
```

Run the application:

```
python main.py
```

In your web browser, enter the following address:

```
http://locahost:8080
```

Use a Nginx as front-end:

```
apt-get install nginx -y
rm /etc/nginx/sites-enabled/default
cp nginx/helloworld.conf /etc/nginx/sites-enabled/
/etc/init.d/nginx restart
```