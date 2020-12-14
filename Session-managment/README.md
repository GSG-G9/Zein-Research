## Sessions management :-
 # what are sessions?
  - in computer science, we define them as (and in simple words) a connection between two devices, systems, webpages or any two sides in the technical world where the two of them exchange information, data, resources, maybe political secrets ...(I'm looking at you FBI)
  - in Universal Analytics, it's defined as a group of user interactions with your website, practically the same but a bit more specific than what we said above.
  - once the connection is no more needed it's closed and everything related to it is (naturally) deleted
  - originally, sessions are all stateful, one of the communication parties needs to keep track of the session data.

 # How to manage sessions in express?
  - we need to install the [express-session](https://www.npmjs.com/package/express-session) from npm
  - here is a [GitHub](https://github.com/expressjs/session) with steps specified on how to use session middleware with express.

  ` const session = require("express-session")
    const app = express();
    
    app.use(session{
        secret: "our secret string",
        cookie: {
            name: "Add a Name Here",
            secure: true
            }
    })
    `