# Smart City Platform: Distributed Nodes

The Smart City Platform is a distributed system that runs on public nodes hosted by anyone. Everyone running public nodes will receive payment from anyone using the distributed system, for needs such as storage, communication and more.

These nodes are different from the public blockchain nodes on the City Chain. The distributed nodes software might be the same as City Chain nodes (daemons) or it might be different. Future investigation is needed for this architecture decision.

The naming might also need to be something that is distinct from the existing City Chain full nodes.

## Payment for services

When a user utilized the services provided by the participants in the distributed nodes network, they will be performing payment to all members of the network. These payments are automatic, and users will need to have wallets with CITY balance to perform (automatic) payment for services utilized.

## Example: Identity Metadata

When an actor want to perform a payment using City Hub, they will be able to see public metadata for the receiver, which can be any user, or merchant. This can be used to increase the trust when performing payments, validating that receiver of the payment before final confirmation (signing).

A user/merchant can at any time, withdraw their published metadata. If the data was stored on the blockchain, it wouldn't be removeable. On the distributed network, data can be replaced/updated and removed.

