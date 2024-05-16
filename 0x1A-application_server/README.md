# Application server

This was the application deployment project for our AirBnB clone. In this
project, I configured Nginx on the web servers provided me by Holberton School
to serve a WSGI Flask app running through Gunicorn. Additionally, I set up an
Upstart script to keep the application running on server reboots.

## Tasks :page_with_curl:

* **0. Set up development with Python**
  * In this task, I configured the file  from my
  [AirBnB_clone_v2](https://github.com/bdbaraban/AirBnB_clone_v2) to serve content
  on the route , running on port .

* **1. Set up production with Gunicorn**
  * This task involved setting up a production environment, installing and configuring
  Gunicorn to serve the same file from task 0.

* **2. Serve a page with Nginx**
  * [2-app_server-nginx_config](./2-app_server-nginx_config): Nginx configuration file
  proxying requests on the route  to the Gunicorn app running on
  port .

* **3. Add a route with query parameters**
  * [3-app_server-nginx_config](./3-app_server-nginx_config): Nginx configuration file
  proxying requests on the route  to the
  Gunicorn app running on port .

* **4. Let's do this for your API**
  * In this task, I configured the API from my [AirBnB_clone_v3](./https://github.com/Ostoyae/AirBnB_clone_v3) to run on Gunicorn.
  * [4-app_server-nginx_config](./4-app_server-nginx_config): Nginx configuration file
  that proxies requests on the AirBnB API to the corresponding Gunicorn app.

* **5. Serve your AirBnB clone**
  * In this task, I configured the complete AirBnB app from [AirBnB_clone_v4](https://github.com/bdbaraban/AirBnB_clone_v4) to run on Gunicorn and be served through Nginx.
  * [5-app_server-nginx_config](./5-app_server-nginx_config): Nginx configuration file
  configured to serve the static assets from  on the Gunicorn AirBnB
  app.

* **6. Deploy it**
  * [gunicorn.conf](./gunicorn.conf): Configuration file for an Upstart script that starts a
  Gunicorn process bounded to port 5003 that serves the content from task 5.
  * The Gunicorn process spawns three worker processes and logs errors to ,
  access to .

* **7. No service interruption**
  * [4-reload_gunicorn_no_downtime](./4-reload_gunicorn_no_downtime): Bash script that gracefully
  reloads Gunicorn.
