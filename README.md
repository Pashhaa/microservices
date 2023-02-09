## Team (#4):

## How to install (Minikube):
1) Make sure Minikube is installed: https://minikube.sigs.k8s.io/docs/start/
2) Start Kubernetes with `minikube start`
3) Enable Ingress addon with `minikube addons enable ingress`
4) Prebuild Docker images with `chmod +x docker.sh && ./docker.sh`
5) Apply k8s configurations with `kubectl apply -R -f k8s`

## How to run (Minikube):
1) Start tunnel using `minikube tunnel`
2) Access frontend on http://localhost

## API Requests

### Auth
`GET /api/auth/me - Get authenticated user`

`POST /api/auth/login - Login user`

`POST /api/auth/signup - Signup user`

### Orders
`GET /api/orders - Get all orders`

`GET /api/orders/get/{orderId} - Get order by id`

`POST /api/orders/create - Create order`

`PUT /api/orders/update/{orderId} - Update order by id`

`DELETE /api/orders/delete/{orderId} - Delete order by id`

### Customers
`GET /api/customer - Get all customers`

`GET /api/customer/{id} - Get customer by id`

`POST /api/customer - Create customer`

`PUT /api/customer/{id} - Update customer by id`

`DELETE /api/customer/{id} - Delete customer by id`

### Warehouse
`GET /api/warehouse - Get all items in warehouse`

`GET /api/warehouse/get/{id} - Get item in warehouse by id`

`POST /api/warehouse/create - Create item in warehouse`

`POST /api/warehouse/update/{id} - Update item in warehouse by id`

`DELETE /api/warehouse/delete/{id} - Delete item in warehouse by id`