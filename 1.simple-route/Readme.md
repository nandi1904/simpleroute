# How to run the application: 

```
env FLASK_APP=./src/simple-api.py flask run    
```

# How to run API Tests:

```
pytest --log-format="%(asctime)s %(levelname)s %(message)s" \
	   --log-date-format="%Y-%m-%d %H:%M:%S" \
	   --html=test-report.html
```

## Run in virtual env

# To run the python server:
1.
python3 -m venv env
2.
source env/bin/activate
3.
pip install -r requirements.txt
4.
python server.py




# Docker 

1. Create the Dockerfile with 
- dependencies
- add the command for bringing up the server

2. Create image
docker build -t "simple-route-1" .

3. Bringup the container
docker run -p 5001:5000 "simple-route-1"

