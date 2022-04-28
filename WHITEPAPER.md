City Chain: White Paper
-----------------------

Updated: **April 16, 2019**   
Version: **Draft 3**   

This whitepaper is our Software Architecture Document. This is a living document that is updated as implementations of features and services are completed, and as the architecture and implementation changes.

**ABSTRACT:** City Chain and the Smart City Platform are a new blockchain and platform granting users access to city services and citizenry information. Cities and citizens will be able to use City Chain to improve how we communicate, socialize, trade and manage our assets (both physical and digital.) In addition, it will be possible to reduce costs and overhead for both citizens and cities.

**DISCLAIMER:** This City Chain White Paper is for discussion and informational purposes only. The information contained herein is subject to change. No part of this draft document is legally binding or enforceable. City Chain Foundation and the City Chain developers do not guarantee the accuracy of or the conclusions reached in this white paper, and this white paper is provided “as is.” City Chain Foundation and the City Chain developers do not make and expressly disclaims all representations and warranties, express, implied, statutory or otherwise, whatsoever, including, but not limited to: (i) warranties of merchantability, fitness for a particular purpose, suitability, usage, title or noninfringement; (ii) that the contents of this white paper are free from error; and (iii) that such contents will not infringe third-party rights. City Chain Foundation, City Chain developers and its affiliates shall have no liability for damages of any kind arising out of the use, reference to, or reliance on this white paper or any of the content contained herein, even if advised of the possibility of such damages. In no event will the City Chain Foundation, City Chain developers or its affiliates be liable to any person or entity for any damages, losses, liabilities, costs or expenses of any kind, whether direct or indirect, consequential, compensatory, incidental, actual, exemplary, punitive or special for the use of, reference to, or reliance on this white paper or any of the content contained herein, including, without limitation, any loss of business, revenues, profits, data, use, goodwill or other intangible losses.

- [Introduction](#introduction-by-chief-technology-officer)
- [Background](#background)
- [What does it solve](#what-does-it-solve)
- [Consensus Algorithm \(PoS\)](#consensus-algorithm-pos)
- [Accounts and identities](#accounts)
  * [Identities](#identities)
- [Payments](#payments)
  * [Send by e-mail](#send-by-e-mail)
  * [Send by SMS](#send-by-sms)
  * [Send by NFC](#send-by-nfc)
- [Wallets](#wallets)
- [City Hub](#city-hub)
  * [Secure Community](#secure-community)
  * [Contacts](#contacts)
  * [Merchants](#merchants)
  * [Voting Framework](#voting-framework)
  * [Property Registry](#property-registry)
  * [Vehicle Registry](#vehicle-registry)
  * [Insurance](#insurance)
  * [\(Smart\) Contracts](#smart-contracts)
  * [Subscriptions](#subscriptions)
  * [Certifications](#certifications)
- [Tools](#tools)
  * [Block Explorer](#block-explorer)
  * [Network Statistics](#network-statistics)


# Introduction

<img src="img/city-chain-gold-thumb.png"
     alt="City Hub" 
     align="right"
     style="float: right; margin-left: 10px;" />

We believe in improving every citizen's quality of life. That is why we are building City Chain and the Smart City Platform.

The promises of Bitcoin, blockchain and other cryptocurrencies are not being fully realized in today's society. This is primarily because the existing systems of economics and trade are tied to fiat currencies, money that is produced and controlled by governments and central banks.

While there are millions of people that hold Bitcoin today, their utilization of it is limited. Most usage requires the exchange from Bitcoin to a local fiat currency that is accepted by a merchant. Gift cards, credit cards and other solutions do help to improve this by allowing consumers to more directly exchange digital money for goods and services without an implicit exchange to fiat currency.

We believe that to realize the full potential of Bitcoin and blockchain technology we need to build solutions that work for everyone, are simple to understand, easy to use, and help both consumers and merchants alike.

We also believe that we need to start building new cities to fully implement blockchain technology. These new cities will have a more open and free policy of monetary exchange from the ground up. Most current states have laws that require the acceptance and usage of their fiat money. We think that competition and freedom is the way forward to find the most optimal solutions for money. We want not only a free market of goods and services, but also of money.

City Chain is both a blockchain technology and a chain of private cities. We are building City Chain and the Smart City Platform to enable new private startup cities to have the tools they need to increase development speed, and reduce costs of planning and operating the city.

The first application of City Chain is the City Coin (CITY) cryptocurrency.

**Sondre Bjellås**   
Chief Technology Officer, City Chain Labs


# Background

The concept for City Chain came about during the planning and development of Norway's first private city, Liberstad. As we started working on the development of the city we realized that we wanted to provide an optimized platform for city operations and citizen interactions.

# What does it solve
There are currently technical hurdles to getting the average individual interested in the concept and usage of cryptocurrencies. Also, there is huge potential to improve the experience of being a citizen through the implementation of blockchain solutions. Current city services are often slow, confusing, and inefficient. 

In order to encourage global widespread usage of blockchain technology, it has to become the foundation and the preferred means of transaction for the majority of people. To achieve this goal, City Chain will develop solutions that improve and enable:

- Merchants to quickly and easily accept cryptocurrencies as a payment method.
- Citizens to quickly and easily perform payments to friends, family, associates and merchants.
    * Payments should be possible using e-mail (P2M/P2MPH), SMS (P2PN/P2SMS), NFC, and using contact list without knowing, sharing or pasting any addresses.
    * Perform payments with on-the-fly currency conversion.
- Full overview and management of investments and assets (digital and physical)
- Management of certifications, the uploading of third party certificates and signing them for digital verification.
- Property registry and details about owned land.
- ...and much more, please refer to the [website](https://www.city-chain.org/) for more details.

# Consensus Algorithm (PoS)
City Chain utilizes Proof-of-Stake as oppose to Proof-of-Work (Bitcoin). We do this for a number of reasons:

* Reduce the demand for electric energy and hardware investments for stakers ("miners").
* Deterministic block interval.
* Avoid competition with Bitcoin and other blockchains for the available PoW-hashpower.

City Chain uses version 3 of PoS. City Chain commits to following the development of PoS consensus algorithms and performing upgrades and modifications in the future. This may result in soft- and/or hard-forks. Modifications to the PoS algorithms will be done to ensure the stability, safety and security of the blockchain-network.

# Accounts

Accounts on the City Chain and Smart City Platform work the same as most blockchains today. By relying on a 12 word recovery phrase (mnemonic) which will act as the seed for derived private/public key pairs, you can access all your data, coins, and information.

# Identities

The platform allows anyone to create their own identities for use in all interactions on the platform and in online and offline commerce. One need not use their legal birth name. You are the source of your identity, and what you identify as is up to you. You can have a single identity, or multiple.

The identity you create on the platform will build up trust over time. Trust will become more and more important in the digital space moving forward. 

We plan to support the [Decentralized Identifiers](https://w3c-ccg.github.io/did-spec/) (DIDs) specification, including implementation of Universal Resolver, Universal Registrar, and Identity Hubs. By implementing these open specifications, you can potentially use your identity on the City Chain to authenticate across multiple decentralized blockchains and systems.

Integration with other blockchains is planned for the identity framework, including Keybase.io.

# Payments

Performing payments on the platform will be possible in as many ways and forms as possible in order to increase adoption and usage. We will be implementing some innovative ideas such as sending funds by e-mail.

## Send by e-mail

The concept is that from within the City Chain wallet or the City Hub a user should be able to send funds using the recipient’s email address. When sending by e-mail, it should be possible to add a PIN/password as an additional security factor, but this shouldn't be a requirement for smaller payments.

When a person receives the funds by e-mail, they will be welcomed with easy to follow instructions on how to get started with City Chain and how to transfer the funds to their newly created account.

If a new user is created and their e-mail address is added to the identity created, friends, family and contacts will in the future be able to perform transfers directly without going through e-mail, which is less secure.

We are considering two methods, P2M ("Pay to e-Mail") and P2MPH ("Pay To e-Mail Public Hash"), where the form is using the contact registry, while the second is more of an e-mail based banking, similar to P2SMS.

## Send by SMS

P2PN and P2SMS are two methods we want to implement for sending funds by SMS.

The first one is "Pay To Phone Number", which relies on the platform contact registry to find the address of a person who is either in the contact registry of the person sending funds or is someone who has chosen to publicly expose some of their contact information.

The second payment method, "Pay To SMS Public Key Hash", is a method to perform payments over SMS, which is a form of banking service through SMS, where the user doesn't need to be using any other part of the platform.

## Send by NFC

We plan to add NFC payment support for our mobile wallet app. Security is important, so this will likely be implemented with payment limits over NFC with a separate funding address where the user can pick the maximum limit. Auto-refund of NFC addresses is also something we will consider.

NFC payments should be possible between two mobile users, and between consumers and merchants that use a City Chain compatible PoS (Point-of-Sale) terminal.

# Wallets

City Hub will be the primary wallet for City Chain. We will be working with third party wallets to enable support for City Coin, but the City Hub will be the preferred app to fully utilize the City Chain and Smart City Platform. 

Other third party wallet apps give users the basic needs to perform transactions and other related tasks. The full set of City Chain and Smart City Platform functionality is accessible through the City Hub.

# City Hub

<img src="img/City-Hub-3d-dark-thumb.png"
     alt="City Hub"
     align="right"
     style="float: right; margin-left: 10px;" />
     
The City Hub is the one-stop-app where citizens, merchants and others can access an overview of everything related to their data on the City Chain and the Smart City Platform.

City Hub is a HTML-based front end built on Angular.

A user who runs the full node edition of City Hub will be able to earn some fees from sharing a configurable amount of disk storage for encrypted data on the Smart City Platform.

City Hub supports different usage modes. Desktop and mobile support is coming in a future update.

- Mobile - Mobile optimized, released to app stores on Android and iOS.
- Light - Light node UI that does not require download of full blockchain.
- Full - Full node UI that supports staking and does a complete verification of the blockchain.
- Point-of-Sale (POS) - Merchant UI optimized for touch screen usage.
- Read-only - A more secure mode that allows you to see all your data without using your private key.

## Secure Community

We believe it is important for citizens to have the ability to communicate freely without having anybody able to listen in on conversations. Whether it’s a conversation between a doctor and patient, a citizen and municipality, or friends and family, the right to privacy is crucial in modern life. 

Today, much communication takes place through email, social media, and custom platforms such as medical and government systems. Often these are hosted by global corporations, and citizens have little to no insight into how their data is being stored and used.  

The Secure Community on City Chain provides end to end encryption with no ability for anyone to listen in on conversations. This functionality relies on modern technologies available on the latest and most secure web browsers. 

What differentiates the City Chain Secure Community from other encrypted communication solutions is that the information is never stored on any device besides that of the user. By paying a small fee, a community can use full nodes to store encrypted archives. 

## Contacts

One of the biggest hurdles for cryptocurrencies is the lack of a contact registry where a user can easily send funds to people already in their address books and make their address publicly available. 

The Contact registry will give citizens full control over what data they want to share, and how it is shared. 

## Merchants

The Merchant framework is one of the most important parts of City Chain, and the future of cryptocurrencies as a whole. In order for cryptocurrencies to be used, merchants need to be willing and able to accept them. 

City Chain plans to deliver complete solutions to merchants that are simple to set up. 

The platform will enable just about anyone to become a merchant and sell goods and services both online and offline. It will also allow existing merchants to improve their sales and customer experiences. The framework will support receipt of payment in the merchant’s currency of choice, including local fiat currency, or even a mix of currencies. 

Integrations with existing ecommerce frameworks will be added, allowing merchants to easily integrate into the Smart City Platform while continue to use existing software for online sales.

Merchant registry will be part of the merchant framework, allowing citizens to discover the merchants available in various cities. Citizens will be able to see what services are provided, and how payments can be made. They will also be able to view transaction history with merchants they have visited.  

## Voting Framework

The ability to vote as either a citizen or an employee is a crucial part of modern society. A voting framework will be part of the Smart City Platform, which will enable anyone to create voting polls that are transparent, secure, and anonymous (if needed.) The exact voting structure will be configurable by the user. 

This voting framework will be used by the Liberstad Incubator Program (LIP,) to allow investors to vote on suggested applications to the incubator program. It will also be used by the City Chain Foundation, allowing individuals who hold City Coins to vote on issues, suggestions and more.

## Property Registry

The Smart City Platform will allow users to register and view their properties on the blockchain, most likely through integrations with existing services. 

A few governments have already started using blockchain for property registrations. The key feature is for citizens to be able to easily see all the details of their properties on the platform. 

## Vehicle Registry

As a vehicle owner you will be able to register on the City Hub. The platform will integrate with VINchain and/or carVertical to ensure that you have access to all relevant details and history of your vehicles. 

## Insurance

Insurance is an important part of modern society, helping individuals, families and businesses handle the unforeseen.

There are blockchain based insurance platforms under development. The Smart City Platform will be built to integrate these platforms, allowing citizens to get insurance coverage easily. Two potential platforms for insurance integration are Etherisc and Insurepal. 

## (Smart) Contracts

The Smart Contracts module gives users an overview of all blockchain based contracts they have enacted. One can additionally upload and safely store copies of non blockchain contracts. 

The Smart Contracts module gives users an overview of all blockchain based contracts they have enacted. One can additionally upload and safely store copies of non blockchain contracts. 

## Subscriptions

Life in the city often involves paying for recurring subscriptions. The Subscriptions module on the Smart City Platform allows users to view all their current subscriptions, including both city services and other merchants. 

Currently, citizens don’t have easy access to view and control all of their subscriptions. They must remember every subscriptions and login to individual websites, and some subscriptions don’t even provide this option.

The other valuable aspect of the Subscriptions module is the ability to view all possible subscriptions in one’s local area and beyond. Examples of subscriptions include waste services, water services, public transportation, bicycle or car rental, car sharing, and more.   

## Certifications

Digitizing and verifying academic credentials will be part of the platform. Corporations will be able to validate potential employees, and public and private educational institutions will be able to give cryptographically verifiable certifications. 

# Tools

While the majority of software functionality developed on City Chain will be part of either the City Chain blockchain or the Smart City Platform and City Hub, there will be certain tools that stand alone. These tools will add additional value to the City Chain ecosystem. 

## Block Explorer

City Chain Labs has launched an official block explorer. We plan to contribute to various existing block explorers to ensure that they integrate well with the City Chain blockchain.

The explorer provides details such as circulating supply, total supply, current market prices, and more. 

[https://explorer.city-chain.org/](https://explorer.city-chain.org/)

## Get started

Visit the following website to quickly learn about and get started using City Chain.

[https://start.city-chain.org/](https://start.city-chain.org/)

## Network Statistics

Based on Grafana, InfluxDB and a specialized version of the full node client, we'll develop a network statistics solution that is similar to [Statoshi](http://statoshi.info/) and [P2SH](https://p2sh.info/).

## Version History

- Draft 3: April 16, 2019
- Draft 2: February 6, 2019
- Draft 1: July 27, 2018
