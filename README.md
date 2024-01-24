1. Project Title

HTTP Caching Proxy Service


2. Description

a. The http proxy - a sercer whose job is forwarding request to the origin server on behalf of the client. 

b. The proxy support GET, POST, and CONNECT request methods.

c. Responses are cached to GET requests, following the rules of expiration time and re-validation in determining if the proxy can serve a request from its local cache or re-fetching from the origin server.

d. Supported multiple concurrent requests by utilizing multiple threads. (Cache shared between all connections and properly synchronized).

e. Clients are able to configure their brower to use this proxy and browse webpages.

f. Kept understandable log containing information about each request.


3. Prerequisites

Install docker


4. Proxy Installation

sudo docker-compose up


(if run.sh file doesn't have the necessary permissions to execute ----- try below:

a. chmod +x run.sh //setting the executable permission for the file

b. docker-compose build //rebuilding the image

c. docker-compose up)


5. Usage

a. Configure "manual proxy configuration" in broswer(Firefox).

b. Use curl
