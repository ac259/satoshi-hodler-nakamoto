# satoshi-hodler-nakamoto
My attempt of building the bitcoin from scratch. I wrote this to better understand the "Bitcoin" and Nakamoto Consensus. This implementation is based on the initial whitepaper *Bitcoin: A Peer-to-Peer Electronic Cash System* by *Satoshi Nakamoto* [[link](https://bitcoin.org/bitcoin.pdf)]

## Components
* Coin <br/>
Chain of digital signatures, transfer of a coin - digitally sign `previous transaction + public key of next owner`.

* Time Stamp Server <br/>
taking a hash of a block of items to be timestamped and broadcast the hash to the network.

* Proof of Work <br/>
Hash Puzzle that is computationally expensive.

* Block <br/>

* Nodes and Miners <br/>

* Merkle Trees - Hash Trees for transaction  <br/>

* UTXO *Unspent Transaction Output* <br/>
This term was not used in the white paper however, this is the same as `section 9: Combining and Splitting Value` in the paper.

* Mining <br/>
Circulation of coins 

* Nakamoto Consensus <br/>

* Limits <br/>
	- [ ] Maximum number of coins
	- [ ] Limiting the number of blocks produced
	- [ ] Mining incentives

* Network 