# xcsi
Stands for Cross chain settlement instruction

The aim of the lab is to create a cross chain settlement instruction. Many chains for issuing and trading digital assets and holding digital cash are being built. We envision a future in which chains are built on multiple platforms. To create a digital market, a chain that holds and trades assets needs to be connected to an accessible payment leg. Trading of assets could happen on one chain and payment could happen at a different venue. Cross chain settlement instructions are needed from the asset trading chain to the payment settlement chain. 

We are transport agnostic. All message encryption as well as at rest (if needed) is outside the scope of this lab.

## Important Ideas
The message is free-standing. Just the contents of the message is enough to make sense. This is in both in terms of the data itself as well as the cryptographic integrity. More similar to the concept of credentials. External witnesses are important, 1. public cryptographic integrity related to identity (DPKI etc.) 2. A way to agree on what is being transacted (the assets, the payment rails) using a public "registry" or a discovery mechanism.
A serialization/deserialization component is needed for conversion into a true human readable document as well as to convert from a human readable doc into a JSON doc which can be transported across. Hashing could include both parts separately and together. This has to be researched.

## Structure

JSON files that define the message are in src/json
Documentation in doc

## License
License file is found in this directory. Apache 2.0 operates for code and CC by 4.0 for all other contributions.


## Maintainers 

Vipin Bharathan vipinsun@gmail.com 
Mani Pillai mani@swapshub.com
Jagdeesh Babu jaga@swapshub.com


