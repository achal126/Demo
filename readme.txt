Hyperledger Fabric: one of the blockchain projects within Hyperledger

private and permissioned


members are enrolled through a trusted membership provider

Two cheif components

Ledger= World State + transaction logs
World state holds the current state 
Transaction logs record the before and after values of the ledger database being used by the blockchain network.

Smart Contracts 

are written in chaincode in go.
Claim that chaincode can be written in other popular languages but not yet implemented.

digitial identity encapsulated in an X.509 digital certificate

For an identity to be verifiable, it must come from a trusted authority. A membership service provider (MSP) is how this is achieved in Fabric. 

The default MSP implementation in Fabric uses X.509 certificates as identities, adopting a traditional Public Key Infrastructure (PKI) hierarchical model (more on PKI later).

was defined in memberserv in v0.6

Public Key Infrastructure (PKI)

There are four key elements to PKI:

Digital Certificates
Public and Private Keys
Certificate Authorities
Certificate Revocation Lists

Fabric provides a built-in CA component to allow you to create CAs in the blockchain networks you form. 

creating channels kinda like realm in Hashgraph

Hyperledger Fabric has been designed to allow network starters to choose a consensus mechanism that best represents the relationships that exist between participants.

Consensus is a pluggable module in Hyperledger.

Solo Orderer: The solo orderer is intended to be an extremely easy to deploy, non-production orderer. It consists of a single process which serves all clients, so no `consensus' is required as there is a single central authority. There is correspondingly no high availability or scalability. This makes solo ideal for development and testing, but not deployment. The Solo orderer depends on a backing raw ledger.

CA is certificate Authority

a Membership Service Provider (MSP) comes into play — it identifies which Root CAs and Intermediate CAs are trusted to define the members of a trust domain, e.g., an organization,

Peers are a fundamental element of the network because they host ledgers and smart contracts. Recall that a ledger immutably records all the transactions generated by smart contracts. Smart contracts and ledgers are used to encapsulate the shared processes and shared information in a network, respectively. These aspects of a peer make them a good starting point to understand Hyperledger Fabric network.



