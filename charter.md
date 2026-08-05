# DRAFT Charter: PTTH Working Group

The PTTH (Protocol for Transposed Transactions over HTTP) Working Group is
chartered to define a standardized mechanism for reversing the roles of HTTP
clients and HTTP servers in a secure and interoperable way. This enables the
creation of connections where the transport interactions are initiated by the
entity that acts in the HTTP server role.

In HTTP deployments, the client initiates requests and the server responds.
However, a growing set of use cases such as dynamic service hosting, edge
computing, NAT traversal, privacy-preserving architectures, and
application-layer rendezvous benefit from having the entity in the HTTP server
role be the one to initiate a transport-layer connection. PTTH allows such
"transposed" transactions, where a transport-layer client can act as an HTTP
server and a transport-layer server can act as an HTTP client. That way, the
transport-layer client can receive HTTP requests from a transport-layer
server and respond to them, under explicit agreement and control.

The PTTH protocol will reuse existing HTTP concepts and designs wherever
possible. The protocol will define how one endpoint can indicate its
willingness to receive HTTP requests from the remote peer, how such requests
are carried, and how security and interoperability are maintained.

## Scope

The working group will produce a (or a combination of) standards-track
specification(s) that define(s):

* A protocol mechanism to enable a transport-layer client to receive HTTP
requests from a transport-layer server and respond to them
* How a proxy authenticates workers
* How a proxy might decide to route a given request to specific workers
* Compatibility and applicability to existing HTTP versions
* Optionally, guidance for implementation and deployment in diverse
environments

## Out of Scope

* Changing HTTP semantics
* Developing mechanisms for reversing application-layer protocols other than HTTP
* Specification of usage-specific signaling or policy frameworks (though such
frameworks may use PTTH once standardized)
* Developing locator mechanisms for transport-layer server discovery
* Developing new transport protocols or extending existing ones
* Protocol mechanisms for requesting additional capacity from transport-layer
clients/HTTP servers
* Defining new identity mechanisms

## Milestones

* Working Group adoption of an initial draft specification
* Working Group Last Call
* Submission to the IESG for publication as a Proposed Standard

## Liaison

The PTTH Working Group will coordinate closely with the HTTP Working Group
(HTTPBis), to ensure architectural alignment with existing and future versions
of HTTP. The group will also liaise with the W3C Technical Architecture Group
(TAG).
