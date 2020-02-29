# satoshi-hodler-nakamoto
My attempt of building the bitcoin from scratch. This implementation is based on the initial whitepaper *Bitcoin: A Peer-to-Peer Electronic Cash System* by *Satoshi Nakamoto* [[link](https://bitcoin.org/bitcoin.pdf)]

## Components
* Coin
Chain of digital signatures, transfer of a coin - digitally sign `previous transaction + public key of next owner`.

* Time Stamp Server
taking a hash of a block of items to be timestamped and broadcast the hash to the network.

* Proof of Work
Hash Puzzle that is computationally expensive.

* Nodes and Miners

* Merkle Trees - Hash Trees for transaction 

* UTXO *Unspent Transaction Output*
This term was not used in the white paper however, this is the same as `section 9: Combining and Splitting Value` in the paper.

* Mining 
Circulation of coins 

* Limits 
	- [ ] Maximum number of coins
	- [ ] Limiting the number of blocks produced
	- [ ] Mining incentives

* Network 