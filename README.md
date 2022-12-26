I have used [Ege Aksoz's](https://github.com/egeaksoz/fullstackapp) repository and his articleas as a starting point. Thank you!

## INSTRUCTIONS

### Create backend image

Navigate to backend folder and type:

``` docker build -t mohammad67/fullstack__backend:TAG . ```

Push the image to my local docker-hub repository:

``` docker push mohammad67/fullstack__backend:TAG ```


### Create frontend image

Navigate to frontend folder and type:

``` docker build -t mohammad67/fullstack_frontend:TAG . ```

Push the image to my local docker-hub repository:

``` docker push mohammad67/fullstack_frontend:TAG ```

It is good practice to tag the images for later tracking the deployment versions.

### Deploy kubernetes

Navigate to kubernetes folder and deploy all ConfigMaps, deployments, and services for backend, frontend, and the database components using:

``` kubectl apply -f . ```

Now the application is available from Controlplane on IP_react_service:PORT as:

``` curl http://IP_react_service:PORT ```

Enjoy!
