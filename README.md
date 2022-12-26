I have used the repository [Ege Aksoz](https://github.com/egeaksoz/fullstackapp) and his articleas a starting point. Thank you!

## INSTRUCTIONS

### Create backend image

Navigate to backend folder and type:

``` docker build -t mohammad67/fullstack__backend:TAG . ```

Push the image to my local docker-hub repository:

``` docker push mohammad67/fullstack__backend:TAG ```


### Create frontend image

Navigate to frontend folder and type:

``` docker build -t mohammad67/fullstack_frontend . ```

Push the image to my local docker-hub repository:

``` docker push mohammad67/fullstack_frontend ```

### Deploy kubernetes

Navigate to kubernetes folder and deploy all ConfigMaps, deployments, and services for backend, frontend, and the database components using:

``` kubectl apply -f . ```

Now the application is available from Controlplane on IP_react_service:PORT as:

``` curl http://IP_react_service:PORT ```

Enjoy!
