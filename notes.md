---
title:  Notes and Further Reading
---

## Notes

[^1]: A sophisticated reader may notice that in fact a Bitcoin address is the hash of the elliptic curve public key, and not the public key itself. However, it is in fact perfectly legitimate cryptographic terminology to refer to the pubkey hash as a public key itself. This is because Bitcoin's cryptography can be considered to be a custom digital signature algorithm, where the public key consists of the hash of the ECC pubkey, the signature consists of the ECC pubkey concatenated with the ECC signature, and the verification algorithm involves checking the ECC pubkey in the signature against the ECC pubkey hash provided as a public key and then verifying the ECC signature against the ECC pubkey.

[^2]: Technically, the median of the 11 previous blocks.

[^3]: The Ethereum protocol should be as simple as practical, but it may be necessary to have quite a high level of complexity, for instance to scale, to internalize costs of storage, bandwidth and I/O, for security, privacy, transparency, etc. Where complexity is necessary, documentation should be as clear, concise and up-to-date as possible, so that someone completely unschooled in Ethereum can learn it and become an expert.

[^4]: See the [Yellow Paper](https://ethereum.github.io/yellowpaper/paper.pdf) for the Ethereum Virtual Machine, while also there are many topics in the [Ethereum wiki](https://github.com/ethereum/wiki/wiki), such as implementations and networking protocols. Then for research and possible future implementation there is [ethresear.ch](https://ethresear.ch). Also there is a [phase 1 sharding roadmap](https://ethresear.ch/t/sharding-phase-1-spec/1407/67?) which includes intended changes for Ethereum 2.0, to roll out over the next few years, starting from 2018.

[^5]: Another way of expressing this is abstraction. The [latest roadmap](https://ethresear.ch/t/sharding-phase-1-spec/1407/67) is planning to abstract execution, allowing execution engines to not necessarily have to follow one canonical specification, but for instance it could be tailored for a specific application, as well as a shard. (This heterogeneity of execution engines is not explicitly stated in the roadmap. There is also heterogeneous sharding, which Vlad Zamfir conceptualized.)

[^6]: Internally, 2 and "CHARLIE" are both numbers, with the latter being in big-endian base 256 representation. Numbers can be at least 0 and at most 2<sup>256</sup>-1.



## Further Reading

1. Intrinsic value: http://bitcoinmagazine.com/8640/an-exploration-of-intrinsic-value-what-it-is-why-bitcoin-doesnt-have-it-and-why-bitcoin-does-have-it/
2. Smart property: https://en.bitcoin.it/wiki/Smart_Property
3. Smart contracts: https://en.bitcoin.it/wiki/Contracts
4. B-money: http://www.weidai.com/bmoney.txt
5. Reusable proofs of work: http://www.finney.org/~hal/rpow/
6. Secure property titles with owner authority: http://szabo.best.vwh.net/securetitle.html
7. Bitcoin whitepaper: http://bitcoin.org/bitcoin.pdf
8. Namecoin: https://namecoin.org/
9. Zooko's triangle: http://en.wikipedia.org/wiki/Zooko's_triangle
10. Colored coins whitepaper: https://docs.google.com/a/buterin.com/document/d/1AnkP_cVZTCMLIzw4DvsW6M8Q2JC0lIzrTLuoWu2z1BE/edit
11. Mastercoin whitepaper: https://github.com/mastercoin-MSC/spec
12. Decentralized autonomous corporations, Bitcoin Magazine: http://bitcoinmagazine.com/7050/bootstrapping-a-decentralized-autonomous-corporation-part-i/
13. Simplified payment verification: https://en.bitcoin.it/wiki/Scalability#Simplifiedpaymentverification
14. Merkle trees: http://en.wikipedia.org/wiki/Merkle_tree
15. Patricia trees: http://en.wikipedia.org/wiki/Patricia_tree
16. GHOST: https://eprint.iacr.org/2013/881.pdf
17. StorJ and Autonomous Agents, Jeff Garzik: http://garzikrants.blogspot.ca/2013/01/storj-and-bitcoin-autonomous-agents.html
18. Mike Hearn on Smart Property at Turing Festival: http://www.youtube.com/watch?v=Pu4PAMFPo5Y
19. Ethereum RLP: https://github.com/ethereum/wiki/wiki/%5BEnglish%5D-RLP
20. Ethereum Merkle Patricia trees: https://github.com/ethereum/wiki/wiki/%5BEnglish%5D-Patricia-Tree
21. Peter Todd on Merkle sum trees: http://sourceforge.net/p/bitcoin/mailman/message/31709140/
