## Stateless vs stateful authentication :-
 # session based authentication (stateful):-
  - the user logs in
  - the server creates a session for the user
  - the session has an id, it's stored on a cookie on (user's)browser
  - the cookie will be sent with every subsequent request as long as the the user in logged
  - the server compares the session id stored in the cookie with the id stored in the server's memory to verify the user
  - a response is sent with the state on whether the user is verified or not.
 # token based authentication (stateless) :-
  - the server creates a JWT with a secret
  - the JWT is sent to the client
  - the client stores it in local storage or in a cookie
  - the client includes it in the header of every request
  - the server validates the JWT with every request and sends a response with the result (if validated you have access, if not the...oops, we have a thief!)

 - the difference here is that the state is not stored in the server but inside the token on the client side.
 - when there is a huge number of people using the system, Scalability becomes a problem in stateful authentication because the session is stored in the server's memory. this isn't a problem with stateless authentication because the token is stored on the client side.
 - cookies work on a single domain or subdomains and are normally disabled by the browser when you work on a cross-domain with stateful authentication so we can't really use different devices but in stateless authentication this isn't a problem because the JWT is in the request header.
 - JWT is bigger in size compared to session ids, it should be considered that only necessary information and nothing sensitive is sent with it.