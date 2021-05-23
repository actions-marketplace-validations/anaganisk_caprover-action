# caprover-action
Action to deploy on Caprover server using doecker.


## Inputs

### `server`

**Required** CapRover server's admin panel URL. Ex. https://captain.root.domain.com.

### `password`

**Required** CapRover admin password. Use ${{ secrets.CAPROVER_PASSWORD }} for better security.

### `appname`

**Required** Application name on the CapRover server. Must exists.

### `docker`

**Required**
Docker image to be deployed.


## Example usage
```
uses: anaganisk/caprover-action@v1
with:
  server: 'https://captain.root.domain.com'
  password: '${{ secrets.CAPROVER_PASSWORD }}'
  appname: 'my-app'
  docker: 'nginx/nginx:latest'
```
