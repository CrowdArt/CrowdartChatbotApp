# Initial code for Udemy course [ChatBots: Messenger ChatBot - DialogFlow and nodejs](https://www.udemy.com/chatbots/?couponCode=GITHUB)


* https://chatbot-facebook1.herokuapp.com/webhook/
* [localtunnel](https://localtunnel.github.io/www/)
* [ngrok](https://ngrok.com/)
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
* heroku addons | grep -i POSTGRES
* heroku addons:create heroku-postgresql:hobby-dev
* [Heroku Data](https://data.heroku.com/)
* npm install --save --save-exact pg
* http://127.0.0.1:59407/browser/
* https://codewithmosh.com/courses/310571/lectures/4881106
* https://developers.facebook.com/apps/254621491907588/messenger/settings/

## REST
The REST architectural style describes six constraints. These constraints, applied to the architecture, were originally communicated by Roy Fielding in his doctoral dissertation (see https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm) and defines the basis of RESTful-style.
The six constraints are: (click the constraint to read more)

Uniform Interface
The uniform interface constraint defines the interface between clients and servers. It simplifies and decouples the architecture, which enables each part to evolve independently. The four guiding principles of the uniform interface are:

Resource-Based
Individual resources are identified in requests using URIs as resource identifiers. The resources themselves are conceptually separate from the representations that are returned to the client. For example, the server does not send its database, but rather, some HTML, XML or JSON that represents some database records expressed, for instance, in Finnish and encoded in UTF-8, depending on the details of the request and the server implementation.

Manipulation of Resources Through Representations
When a client holds a representation of a resource, including any metadata attached, it has enough information to modify or delete the resource on the server, provided it has permission to do so.

Self-descriptive Messages
Each message includes enough information to describe how to process the message. For example, which parser to invoke may be specified by an Internet media type (previously known as a MIME type). Responses also explicitly indicate their cache-ability.

Hypermedia as the Engine of Application State (HATEOAS)
Clients deliver state via body contents, query-string parameters, request headers and the requested URI (the resource name). Services deliver state to clients via body content, response codes, and response headers. This is technically referred-to as hypermedia (or hyperlinks within hypertext).

Aside from the description above, HATEOS also means that, where necessary, links are contained in the returned body (or headers) to supply the URI for retrieval of the object itself or related objects. We'll talk about this in more detail later.

The uniform interface that any REST services must provide is fundamental to its design.

Stateless

Cacheable

Client-Server

Layered System

Code on Demand (optional)

## Promises
Objects used to control flow of deferred and asynchronous operations.
A `Promise` is in one of these states:
* pending: initial state, not fulfilled or rejected
* fulfilled: successful operation
* rejected: failed operation
* settled: the Promise is either fulfilled or rejected, but not pending


curl -X GET "localhost:5000/webhook?hub.ven=my_chatbot_password&hub.challenge=CHALLENGE_ACCEPTED&hub.mode=subscribe"