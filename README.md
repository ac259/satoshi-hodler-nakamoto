# satoshi-hodler-nakamoto
My attempt of building the bitcoin from scratch. I wrote this to better understand the "Bitcoin" and Nakamoto Consensus. This implementation is based on the initial whitepaper *Bitcoin: A Peer-to-Peer Electronic Cash System* by *Satoshi Nakamoto* [[link](https://bitcoin.org/bitcoin.pdf)]

## Components
- [ ] Coin <br/>
	- [ ]Chain of digital signatures - elliptical curve digital signature algorithm [[link](https://github.com/warner/python-ecdsa)].
	 Transfer of a coin - digitally sign [`previous transaction + public key of next owner`]. 
	 Code for a simple `ecdsa`:*(from stackoverflow)* <br/>
	 Usage: <br/>
	 ```import ecdsa
		# SECP256k1 is the Bitcoin elliptic curve
		sk = ecdsa.SigningKey.generate(curve=ecdsa.SECP256k1) 
		vk = sk.get_verifying_key()
		sig = sk.sign(b"message")
		vk.verify(sig, b"message") # True
	```
	<br/>
	To verify an existing signature with a public key: <br/>
	```
	import ecdsa
	message = b"message"
	public_key = '98cedbb266d9fc38e41a169362708e0509e06b3040a5dfff6e08196f8d9e49cebfb4f4cb12aa7ac34b19f3b29a17f4e5464873f151fd699c2524e0b7843eb383'
	sig = '740894121e1c7f33b174153a7349f6899d0a1d2730e9cc59f674921d8aef73532f63edb9c5dba4877074a937448a37c5c485e0d53419297967e95e9b1bef630d'
	vk = ecdsa.VerifyingKey.from_string(bytes.fromhex(public_key), curve=ecdsa.SECP256k1)
	vk.verify(bytes.fromhex(sig), message) # True
	```
- [ ] Time Stamp Server <br/>
taking a hash of a block of items to be timestamped and broadcast the hash to the network.

- [ ] Proof of Work <br/>
Hash Puzzle that is computationally expensive.

- [ ] Block <br/>

- [ ] Nodes and Miners <br/>

- [ ] Merkle Trees - Hash Trees for transaction  <br/>

- [ ] UTXO *Unspent Transaction Output* <br/>
This term was not used in the white paper however, this is the same as `section 9: Combining and Splitting Value` in the paper.

- [ ] Mining <br/>
Circulation of coins 

- [ ] Nakamoto Consensus <br/>

- [ ] Limits <br/>
	- [ ] Maximum number of coins
	- [ ] Limiting the number of blocks produced
	- [ ] Mining incentives

- [ ] Network 