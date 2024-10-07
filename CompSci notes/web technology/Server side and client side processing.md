When using the internet, the majority of interactions involves two connected systems
- the client - user
- the server - server holding web page or resource

when processing interactions between the client and server, decisions are made concerning whether processing is done using the client or server

The decisions are based on
- **performance**
- **security**
- **usability**

## Client side
things processed on the client involve
- Javascript data validation
- manipulation of UI elements
- application of website styles with CSS
the reason that processing is outsourced to the client is that it reduces load on the server, while also reducing web traffic, by reducing data transfers to and from the server

many clients can perform a bulk of processing for the server, at minimal impact to each user

client side processes can be manipulated however, so not all tasks can be outsourced to client computers, for the sake of security

## Server side
things processed on the server involve
- further validation
- Database updates and queries
- data encoding into HTML
- processing of sensitive data
- complex calculations
these things are done on the server to act as a safety net, ensuring that all data entered is valid, ensuring that data is secure, and ensuring that faults can only occur on the client side

complex calculations are run on the server in order to keep the web page running well, as the server is intended for performance while the client's processing power may vary
