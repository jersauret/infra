kong admin on port 8002

typical POST REQUEST to create a service:
curl -i -X POST --url http://localhost:8001/services/ --data 'name=customers-service' --data 'url=http://customers_service'