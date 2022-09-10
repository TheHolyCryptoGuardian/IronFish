# IronFish

Iron Fish is a decentralized, proof-of-work (PoW) based, censorship-resistant, and publicly accessible blockchain project. It is designed to support strong privacy guarantees on every transaction. Similarly to how the invention of the SSL/TLS layer in the '90s paved the way to e-commerce and benefited countless industries, we believe that privacy is a fundamental requirement to protect the user and expand the use of cryptocurrency.

We have designed Iron Fish to be a new cryptocurrency from the ground up to enable easy-to-use, fully-private payments by closely following the Sapling protocol. Every account is equipped with a view key to grant its holder read-only permission for the details of that account.

With this protocol, we are challenging previous patterns of full node usability. The Iron Fish networking layer supports WebRTC with WebSockets, making it trivial for all users to make a true P2P connection with no other setup requirements. Our first Iron Fish implementation is built such that it can be extended to run a full node directly in the browser in future iterations. And our focus is to lower the barrier to entry so that any person with a computer feels comfortable enough to run a full node.

# Introduction

Privacy is controversial, but it shouldn’t be. In fact, privacy leads to innovation — social evolution through changing laws, and the freedom to simply be you. Take doors on houses or passwords for bank accounts, both of which are precautions most people take even though they might say they have nothing to hide.

At Iron Fish, we are building something we’re truly proud of: a cryptocurrency that does not compromise on privacy or accessibility. Digital cash that embodies using privacy for good. We are all moving towards becoming fully digital global citizens where our every activity and purchase is carefully logged, analyzed and sold. In this world, privacy is more important than ever and has growing demand worldwide.

Popular cryptocurrencies like Bitcoin, Ethereum, and others are the least private way of transacting — their protocols fundamentally work on complete transparency to verify transactions. Though other privacy coins exist, they all either lack the privacy guarantees they’ve promised or are so hard to use they barely have any real usage (and oftentimes both).

There is huge untapped potential here — but only if users feel truly protected by their cryptocurrency, and are able to access it. Just like the introduction of SSL/TLS in the '90s opened up the floodgates to e-commerce (the predecessors of HTTPS), we believe that an accessible privacy coin will lead to a new class of industries of borderless products and companies.

In this paper, we cover how Iron Fish works, and why we’ve built it this way. While we endeavor to explain things as much as possible and go over all relevant terminology, some parts will require a basic understanding of elliptic curve cryptography.

# Commands to install [**IronFish node**](https://raw.githubusercontent.com/TheHolyCryptoGuardian/IronFish/main/Node)

Use `wget -q -O ironfish.sh https://raw.githubusercontent.com/TheHolyCryptoGuardian/IronFish/main/Node && chmod +x ironfish.sh && sudo /bin/bash ironfish.sh` to install the node quickly.

Use `journalctl -u ironfishd -f` to check node logs.

Use `systemctl restart ironfishd` to restart the node.

Use `service ironfishd stop` to stop the node.

Use `ironfish config:set enableTelemetry true` to enable telemetry.

Use `ironfish status -f` to check node status.

Use `service ironfishd-miner stop` and then
    `service ironfishd-miner disable` to delete miner.
