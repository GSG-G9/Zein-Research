## Attacks ?!!
 # Man In The Middle :-
  - an attack were the the hacker alters the communication between the two parties. the hacker is actually controlling the whole exchanging making the two parties think they are talking to each other (..but they're not!)
  - how to defend our sessions from this? one way to do this is Authentication: use keys and ids, cookies with encrypted tokens..etc.

 # Cross Site Scripting :-
  - attackers inject client-side scripts  into web pages viewed by other users.
  - one way to protect your system is cookie security, `HttpOnly` makes the cookie unavailable to client-side scripts.

 #Cross Site Request Forgery :-
  - unauthorized commands are submitted from a user that the web application trusts.
  -in other words, an attacker tricks the user into submitting a web request that they did not intend. This may cause actions to be performed on the website, such as:
     1. server data leakage
     2. change of session state
     3. manipulation of a user's account
  - prevention :-
    - Cookie to header token:
        1. web application sets a cookie that contains a random token
        2. front end reads the token and an http header sent with a request to the server
        3. server validates the integrity of the token.