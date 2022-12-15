<h1><p align=center>Koinos (KOIN)</h1>

[Koinos.io](https://koinos.io/) - [CoinGecko](https://www.coingecko.com/en/coins/koinos) - [EtherScan](https://etherscan.io/token/0x66d28cb58487a7609877550e1a34691810a6b9fc) - [Whitepaper](https://koinos.io/whitepaper)</p>

Written by [@fbsloXBT](https://twitter.com/fbsloxbt), September 29th, 2021 

---

<h3>Introduction:</h3>

Update: Koinos Snapshot was taken on October 31st 2022 ([tx](https://etherscan.io/tx/0xf28c62da7a075d42f471527c8305421fba4d964cf3fb9eea0169927b53e9cf03)), ERC20 KOIN token is now worthless and buying KOIN is not possible until main-net launch.

Update: Mainnet launched on 5th November 2022.

Update: KOIN is now listed on MEXC: https://www.mexc.com/exchange/KOIN_USDT

---

Koinos is not a blockchain, it is a blockchain building technology (think Hyperledger, Cosmos, Polkadot) that makes it far faster and easier to launch high performance blockchains with no fees and capable of evolution. Making it far easier for developers to launch their own blockchains.

<sup>Note: Koinos is blockchain framework, while Koinos Mainnet is an implementation of Koinos framework, expected to launch in Q4 2022.</sup>

Koinos Mainnet is fee-less blockchain, utilizing microservice architecture to achieve vertical scalability. All transactions are free, but enforcing proportionate network usage, if you need 1% of network resources, you need to hold 1% of liquid KOIN tokens.

Every aspect of Koinos is WASP (web assembly) smart contract, meaning any feature can be added or upgraded without hard forks, making it the most upgradeable blockchains, capable of rapid evolution and absorption of new technologies (such as new consensus algorithms, scalability techniques…)

Koinos is language agnostic, meaning it can support variety of programming languages (such as C++, TypeScript, Python, Go, etc.), since every contract is compiled to WASP before it’s uploaded to the blockchain, This gives it an advantage since it allows any developer to participate without having to learn new language first (compared to EVM chains that require Solidity/Vyper, Cardano requires Haskell skills…).

KOIN token is fair launch token, launched in October 2020 with PoW mining (using CPU algorithm, making it possible for everyone to mine KOINs). Total supply before launch is 100M, with annual inflation up to 15% after mainnet launch.

One of the main reasons I’m so interested in Koinos (and KOIN) is its low market cap. At the time of writing, it’s sitting at only $12,146,783. In my opinion, this is absurdly low for such project. According to CoinGecko, it’s currently at rank 965, below completely dead projects and scams. It gives it huge upside even if it delivers on half of the promises.

<h3>Team:</h3>

Koinos team is made of 6 blockchain engineers, all of them have previous blockchain development experience. Most of them worked on Steem (as part of Steemit team) blockchain, once top 3 blockchain (before bad leadership ruined it). Steem was one of the fastest & most scalable chains back in 2017. 
I know them since 2017, and I believe they have technical knowledge to build a successful blockchain (and that they aren’t anon scammers like it’s so common for many new projects).

<h3>Technical details:</h3>

To learn more, you can also read full whitepaper here: <https://koinos.io/whitepaper/>

In the early days of blockchains, there was no distinction between application and operating system. Developers had to build their applications from the ground up, since no tools exited yet. For example, Bitcoin is both application (sending money) and operating system (blockchain producing blocks & p2p distributing them). But such system design causes problems, since any upgrades can effect entire applications, and code itself can get very complex and bloated.

Solution for this problem is abstraction of operation system and applications. Example of this is Ethereum, where blockchain is separated from smart contracts running on it. Even if smart contract has bugs, blockchain itself will keep running without issues. But initial issue with upgrading core aspects of the chain remain, any upgrade of the underlying blockchain requires hard fork.

To solve this problem, another layer of abstraction is added, “blockchain BIOS”. It makes upgrades to the blockchain itself much easier, while minimizing downtime. At the base of the Koinos stack is a blockchain framework that features a set of “thunks” that represent blockchain basics like contract input/output, getting parameters, writing to the database, etc. Above the framework is a system call layer that provides library-like support to smart contracts that can be upgraded in-band. System calls can be either thunks (native implementations) or smart contracts (WASM implementations).

![thunks](https://koinos.io/thunks.png)

To increase scalability, StateBD is used. StateDB started as an evolution on chainbase, but has become its own beast entirely, replacing chainbase in the process. On BitShares, Steem, and EOS, the database tracks the most current state. That is the head block state plus pending transactions. This means the database never actually reflects the current state of the blockchain. In order to address that issue, when each block is applied the pending transaction state is undone, the old values are written back to the database, and then the block is applied. One problem with this approach is that most of the time this means performing the exact same calculations again and writing the same state back to the database that was just there which is inefficient.

<h1><p align=center>DISCLAIMER</h1>

<h3>Do Your Own Research</h3>

My (@fbslo/@fbsloXBT) content is intended to be used and must be used for information and education purposes only. It is very important to do your own analysis before making any investment based on your own personal circumstances.

<h3>No Investment Advice</h3>

I (@fbslo/@fbsloXBT) am not a broker/dealer, I am not an investment advisor, I have no access to non-public information about this project, and this is not a place for the giving or receiving of financial advice, advice concerning investment decisions or tax or legal advice. I am not regulated by the Financial Services Authority.

No content on the site constitutes - or should be understood as constituting - a recommendation to enter in any transaction or to engage in any of the investment strategies presented in this content.

<h3>No Reliance</h3> 

Accordingly, I will not be liable, whether in contract, tort (including negligence) or otherwise, in respect of any damage, expense or other loss you may suffer arising out of such information or any reliance you may place upon such information.

<h3>Investment Warnings</h3> 

We would like to draw your attention to the following important investment warnings.

-   The value of investments and the income derived from them can go down as well as up.
-   Investors may not get back the amount they invested - losing one's shirt is a real risk.
-   Past performance is not a guide to future performance.
