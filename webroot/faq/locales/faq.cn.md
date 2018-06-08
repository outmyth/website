### Chia FAQ

+ <b>Q: 什么是Chia？</b>

A: Chia是一个处于上市前阶段的数字货币和区块链，其基于空间证明和时间证明的共识算法，而非传统意义上的工作量证明。Chia的共识机制是让“农民”通过分配不用的存储空间来”耕作“自己的农场，他们通过解决区块难题而获得Chia币。Chia的“耕作” 结合使用了空间证明和时间证明两种共识算法，来降低曾经在基于空间证明的区块链上发生的那些已知的攻击。我们的目标是杜绝通过浪费大量的电力来让区块链变得安全，同时又能缓解中心化的程度（例如ASIC矿机挖矿）。在“播种”过程中，硬盘的空闲空间会被随机生成的工作证明所填充。



+ <b>Q: 耕作是什么意思？</b>

A: Chia的耕作类似于安全地生成区块的挖矿过程。耕作就是对你硬盘上未使用的存储空间进行快照（播种）。根据一位农民可以耕作的存储空间与网络上所有耕作过的存储空间的百分比关系，你应该能够获得跟你愿意用于耕作Chia的存储量相对应的抽奖类型的薪金。你用于耕作的未使用的空间越多，则胜出的几率就越大。购买硬盘来耕作Chia的奖金并不太多，因为Chia预计到那时候周围会有非常多的空闲空间，这不会逐步增加所有者的成本。Chia会利用这些空闲的空间。在这个世界上有如此多的存储空间，对于普通用户而言赢得奖项的几率极低，但是考虑到这只是使用很少的能源和带宽，并且空间都是空闲的，即使给你的奖励很少也不是一个大问题。在Chia的世界里没有矿池，矿工，ASIC矿机和能源浪费。



+ <b>Q: Chia和Bitcoin的主要差别是什么？</b>

A: Chia是利用存储空间（例如硬盘）进行耕作的，而非使用电力进行挖矿。这样会接触到更广泛的普通用户，并极大地降低为让网络更安全而进行发电和定制硬件的消耗／浪费。Chia反对农民的中心化。Chia还会涵盖一整套针对比特币协议的基本优化：
为更好地支持智能交易，万物皆<a href = "https://en.wikipedia.org/wiki/Boneh%E2%80%93Lynn%E2%80%93Shacham">BLS签名</a>，并且它还包含一批　　　bugnd it will include a bunch of bug fixes to things like <a href = "https://bitcoin.stackexchange.com/questions/20597/where-exactly-is-the-off-by-one-difficulty-bug">timewarp</a> while making those fixes available back to Bitcoin. The goal is to make hard forks effectively impossible, so governance will come from user choice and bitcoin-like decentralized incentives.



+ <b>Q: 什么是＂空间证明＂？</b>

"Proof of space" should not be confused with storage. Storage via a blockchain protocol is storage of some data that is directly useful. Proof of storage protocols like Filecoin, MaidSafe, Sia, or Storj require ridiculous amounts of bandwidth and those concepts will not be used in the Chia protocol. Proofs of space are data which is useless for anything but generating proofs of space. Making a proof of space or providing a proof to the network requires essentially no bandwidth. A proof of space can be thought of as a precommitment to keeping some storage unused. Client software will make managing farmed storage easy for farmers as they will have options to incrementally shrink the size of their farm to make room for their useful files as needed.



+ <b>Q: 播种是什么意思？</b>

A: Seeding is a process that requires reading and writing every sector of the allocated farming space more than once; but once a drive is seeded you will be able to farm it for as long as the proofs remain on disk. The initial seeding process fills the farmed space with proofs from random inputs and then runs a sort to make looking up those resulting proofs fast. Drives will be read using low-level direct access APIs. The client will support seeding multiple drives. Re-seeding storage gives no advantage normally. The only reason to reseed a drive is if too many of the existing proofs have been overwritten. Seeding a disk will take significant amounts of time once per drive but the goal is that an average farmer can seed their farmed space in 24 to 48 hours for initial set up.



+ <b>Q: Chia产品何时推出？</b>

A: Chia plans a coin sale in Q2 and a network launch by the end of 2018, but this is not set in stone and is dependent on further development.



+ <b>Q: 我如何购买Chia？</b>

A: Chia plans on doing some kind of sale to the public and we are working with our lawyers at the moment. The goal of our sale is to be as widely available to investors as possible. We need to do some amount of additional fundraising as we're just getting Chia up and running and it would be nice to fund ongoing development and enhancements in the future. There will be a pre-farm of currency whose allocation will be split between being earmarked to fund future development and the team. The funding mechanism and pre-farm amounts will be transparent and available publicly before coin sales commence.



+ <b>Q: 目前Chia开发处于什么阶段？</b>

A: 尚未开始编写代码。数学原语的工作业已完成，目前处于准备出版阶段。 我们现在就在招募程序员，编码工作马上就会开始。关于空间证明和避免Hellman时空折衷的技术论文参见<a href = "https://eprint.iacr.org/2017/893">这里</a>。



+ <b>Q: 何时我就能耕作Chia农场？</b>

A: We hope to have a public sale in Q2 2018, and you'll be able to farm once the network launches which we hope will be before the end of 2018. All dates remain subject to change based on ongoing development.



+ <b>Q: 时间证明是什么意思？</b>

A: Proofs of time are the second step of farming. Proofs of time depend on a function that takes a certain amount of wall clock time to generate a proof, but that proof is canonically correct for the current block and can be quickly verified as correct by anyone in the network. Chia expects there to be a limited number of proof of time nodes as those nodes are not rewarded for coming up with the current block's proof of time. Only the farmer who had the best proof of space from his farm will be rewarded with Chia coin at each block.



+ <b>Q: 为何命名为Chia？</b>

A: "Chia" is the name of a grain you might have heard of before. It's green. It goes with the "farming" theme.



+ <b>Q: 更好的硬盘空间是否就意味着更多的Chia？</b>

A: Your chances of farming the next block are directly proportional to the amount of storage space you allocate to Chia farming.



+ <b>Q: 是否值得购买硬盘来耕作Chia农场？</b>

A: Chia believes that it will be unprofitable to buy hard drives just for the purposes of farming, as everyone will be able to get rewards from unused storage - which there is a lot of. Farming rewards will likely be small, but it isn't costing a farmer anything extra if you already have the storage for some other reason. People have already paid for a lot of unused storage capacity - there's ridiculous excess resources available - so it will be unprofitable to buy storage just for the sake of farming. This is directly related to storage being useful for other things, although it isn't "useful" farming in the sense that the calculation itself isn't productive, but it is leveraging a useful resource. To the extent that Chia unexpectedly drives developments that decrease the cost of storage, we think that's a benefit for society - especially when compared to wasting electricity on custom ASIC mining hardware.



+ <b>Q: Chia跟其他存储相关的币（例如Burst） 有何不同？</b>

A: Burstcoin doesn't have the proof of time component therefore there are attacks that make it unsuitable as a mining algorithm. Additionally, Chia simplifies the math used for proofs of space. Chia also inherits the real world deployment experience of the Bitcoin protocol.



+ <b>Q: Chia将如何进行融资？</b>

A: Chia has raised a seed round of funding but we have enough development work to do that raising funds in the future is necessary to make it happen. We're going to try to do so in a way which is as transparent and open to the public as possible.



+ <b>Q: Chia的交易会有多快？</b>

A: Chia will support Lightning Network out of the box in addition to its blockchain, so payment speed will depend on whether there is an available lightning path. Lightning transactions take less than a few seconds on reasonable network latencies. Our block times for on-chain transactions will be similar to Bitcoin.



+ <b>Q: 还有哪些其他的开发工作呢？</b>

A: After the initial release our focus will be on supporting Lightning as it is today, adding in off-chain channels, supporting MAST and probably <a href = "https://blockstream.com/simplicity.pdf">Simplicity</a> and covenants to support vaults. Chia is going to support atomic swaps out of the gate. We're starting with Bitcoin script using BLS signatures instead of DSA. The plan is to roll releases out in conjunction with Bitcoin rollouts because it's based on the same codebase.



+ <b>Q: Chia会用到哪种脚本语言？</b>

A: We will be going with a modified Bitcoin script for starters and with a switch to BLS signatures. <a href = "https://www.youtube.com/watch?v=Og52VDU-pjc">This talk</a> explains our reasons for both changes. Longer term we will add Simplicity once it's available. We're building on the Bitcoin codebase, so core development will be in C/C++.



+ <b>Q: Chia农场耕作的难度有多大？</b>

A: Like Bitcoin, difficulty will dynamically adjust to keep block times regular. Farming difficulty will balance both the difficulty of proofs of space and proofs of time. As a result, as farming competition goes up, you can expect rewards from a particular amount of storage to go down. We do not expect farming to have a high enough expected value to be worth purchasing drives in order to farm.



+ <b>Q: 硬盘必须要有多大呢？</b>

A: There will likely be a minimum allocation size of 100 GB or 1 TB. It isn't so much to enforce a minimum as to require a minimum amount of wall clock time to pass before an allocation can be done so attackers can't repeatedly generate and try new allocations instead of doing a single lookup.



+ <b>Q: 我能在台式电脑上经营Chia农场否？</b>

A: There will still be some rewards for desktop farmers and the cost will still be effectively zero for some nonzero rewards. It isn't like Bitcoin mining where a desktop loses money mining because of the electricity it's burning and the fact that it's not competitive with ASIC miners. Bandwidth requirements are also expected to be very low.



+ <b>Q: Chia是否采用与比特币类似的容量？</b>

A: There will be three halvings of Chia farming rewards to ultimately get to a low fixed amount of chia rewarded to farmers per block. The coins in circulation continues to increaseat the fixed rate of annual mining but the proportion of coins (grains?) minted (grown?) each year perpetually goes down as a percentage of the total coins in existence. To give a sense of what this means in practice, it will take approximately 153 years for the amount of Chia to double after network launch.



+ <b>Q: Chia如何防范矿工中心化？</b>

A: Chia uses empty storage (like hard disk drives) to farm seeds. As there is so much empty storage space available and anyone with unused storage space will be able to farm, this should lead to farming decentralization. Bitcoin's proof of work mining system drives the formation of blocks toward a limited number of miners because aquiring specialized ASIC mining equipment and locating them near cheap electricity is beyond most people's ability to invest. Manufacturers of storage could optimize storage hardware to farm faster or cheaper, but the cost of doing so is probably not worth the reward and that would otherwise have the benefit of generally decreasing the cost of storage for everyone. Chia should become the most decentralized cryptocurrency on the market.



+ <b>Q: Chia会开源吗？</b>

A: Chia will release academic papers about the building blocks of the protocol, and all implementation code will be open source. We're going to use the <a href = "https://www.apache.org/licenses/LICENSE-2.0">Apache License</a>. There's some chance we'll keep our source code a bit more proprietary when testnet is out but mainnet isn't up yet, but we will definitely license all our source code under the Apache License once mainnet is generally available.



+ <b>Q: 哪里可以读到更多的技术白皮书呢？</b>

A: Instead of just one white paper like most projects, we're going to have academic papers in journals. So far we have <a href = "https://eprint.iacr.org/2017/893">our first paper</a> which was accepted by Asiacrypt and our <a href = "https://eprint.iacr.org/2018/183">second paper</a> which won best paper at Eurocrypt. There will be at least one more paper going over how to hook the whole thing together into a blockchain.



+ <b>Q: 哪里可以找到更多的信息呢？</b>

A: You can sign up for the announcements list to get info as it comes out. Also we're available to discuss announcements on Keybase. Check out our homepage for links.
