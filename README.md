# Acceleration

A set of 3 microservices to calculate the acceleration of an object.

## Prerequsites

1. A kubernetes cluster

2. Ingress controller - Nginx

## How to

### Deployment

1. Clone this repository

2. cd `acceleration`

3. Dry run install
    ```bash
    $ kubectl apply -k . --dry-run=client
    ```

4. Deploy the manifests
    ```bash
    $ kubectl apply -k .
    ```

### Test run

```bash
$ curl "<Host FQDN>/calc?vf=200&vi=5&t=123"
````
