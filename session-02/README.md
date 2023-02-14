# Web Application

Web Application Architecture is divided into 3 components.
- Presentation Layer
- Application Layer
- Data Layer

The Presentation layer will be the UI  where the user interacts and application layer contains business logic for processing and data layer contains data stored in databases.The UI and backend mostly communicates using HTTP.

# How Web Request is Handled

* Now a Days for better accessibility,Web Applications are getting deployed on different CDNs(Content Delivery Network).
* CDN is a distributed server and its main responsibility is to handle the request based on geographical location(contains origin and edge servers) and respond with static content(HTML,CSS,Javascript).When a Web Request is made DNS will resolve the ip address and nearest CDN looks at the cache and if not present it checks with the origin server and caches the data to serve subsequent requests.
* JavaScript client will send requests to server(built using REST) by using different HTTP Methods(GET,POST,PUT,DELETE).The Java Backend handles the incoming request and performs the operations and sends response along with the status code which is then presented in the UI.
* HTTP Protocol is a stateless protocol so it doesn't remember previous requests the server handles this scenario using Cookies.
* The Cookies were sent to UI as response header,the browser stores cookies on the users device and client sends the cookie to server for next requests and server handles accordingly.
