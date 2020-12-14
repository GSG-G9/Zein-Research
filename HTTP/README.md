## How HTTPS works :-
 # first we use Https for 3 things:
  - privacy: i hide my requests from "eavesdropping", from hackers or any third party trying to steal data from me. the lock in the URL bar means that no one is watching over my connections.

  - integrity: there's this thing called man-in-the-middle-attack, it's; simply put: someone interfering between me and the browser and messing the data i'm sending. https helps me save my requests from this attack. it means that my message in not being manipulated on its way to the browser.

  - identification: it means it checks if the requests are sent from an authorized source using a digital signature attached to a message can identify the sender; an (SSL) certificate. it also means that the site that yI'm using is indeed the one you think it is.

 # second, let's talk about TLS/SSL certificates :-
  - SSL stands for 'Secure Sockets Layer'. A protocol created by Netscape.
  - Netscape gave control of SSL protocol to the IETF: Internet Engineering Task Force who released TLS version 1.0 (Which was really SSL 3.1).
  - SSL was renamed to TLS: Transport Layer Security. (CONFUSION).
  - TLC 1.3 was approved in march 2018 brought great security improvements and removed old weaker features.
  - so to conclude: SSL/TLC were created to provide (Security) over networks, request and responses between clients ans servers, it protects communication.
  - historically, it was a war between companies but ended with confusion to browsers and developers. :( 

 # last, how HTTPS actually Works :- 
  1. issues certificates.
  2. confirms the identity of the certificate owner
  3. provides proof that the certificate is valid.
  4. the browser connects to a site via HTTPS and downloads the certificate.
  5. the browser starts reading your certificates and sees it they're all valid and shows that you are trusted with a green lock in th URL bar.

 # How to use certificates in a node project?
  - here is this [GitHub](https://github.com/PatrickKalkman/Developer-SSL-Certificates) that shows you how to generate a certificate for development.