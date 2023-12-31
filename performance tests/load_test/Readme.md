## Load test running
1. Spin up all the servers using `docker-compose up --build`.
2. Run load test using command line: `locust --headless --users 100 --spawn-rate 1 -H http://0.0.0.0:8001` Note `8001` is the port for api end point specified in the corresponding docker file (`src/api/Dockerfile`)
3. You can use the GUI version using `locust`. Make sure you are in the directory `test/load_test/` as `locustfile.py` is present there.

*Run the heavy tests on isolated environments like github codespaces (and not on your local machine).*

<br>

## Benchmarks:
<img width="1257" alt="image" src="../../essentials/locust.png">
- Achieves a response rate of 350ms for 99.9% of the requests at an average of 46 requests per second.
         

<br>          

## References:        

- Locust: [docs](https://docs.locust.io/en/stable/what-is-locust.html)        
