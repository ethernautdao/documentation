---
description: This is a guide for those curious about how to mentor
---

# 🤔 Mentor resources (know more)

Below roadmap can be used as a rough guideline to plan your mentorship. The roadmap should be modified on a per-mentorship base to account for the mentees individual skills and level of knowledge.

### Roadmap <a href="#roadmap" id="roadmap"></a>

* Smart Contract Dev Mentorship
  * Week 1 - 2: Mentee weekly demand 4hs
  * Week 3 - 4: Mentee weekly demand 6hs
  * Week 5 - 4: Mentee weekly demand 12hs
  * Week 6 - 8: Mentee weekly demand 20hs

### Week 1: <a href="#week-1-wb-25th-april" id="week-1-wb-25th-april"></a>

* Set up a regular slot for the weekly call
* Skills gauge to identify areas for improvement/focus
  * Solidity Language
  * EVM
  * Testing Smart Contracts
  * Hardhat
  * Typescript
  * Secure Code
* Study plan with resources
* Daily CTF with GitHub repo explaining solutions. Damn Vulnerable DeFi

### Week 2:  <a href="#week-2-wb-2nd-may" id="week-2-wb-2nd-may"></a>

Depending on the skills gauge.

* Learn common tooling and become comfortable with doing the following:
  * Creating contracts from scratch
  * Deploying contracts using hardhat
    * Check out hardhat deploy and set up the project: [https://github.com/wighawag/hardhat-deploy](https://github.com/wighawag/hardhat-deploy)
  * Verifying contracts with Etherscan plugin
  * Testing contracts with hardhat, typescript & [ethers.js](https://dev.to/yakult/a-beginers-guide-four-ways-to-play-with-ethersjs-354a)
  * Creating GitHub workflows to run tests on commits and PR merges

<- OR ->

* Analyze common DeFi Contracts & make a personal note/blog posts etc detailing how they work
  * [Sushi Masterchef](https://github.com/sushiswap/sushiswap/blob/canary/contracts/MasterChef.sol)
  * [Masterchef V2](https://github.com/sushiswap/sushiswap/blob/canary/contracts/MasterChefV2.sol)
  * [Uniswap V2 Pair](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol)
  * [Uniswap V2 Router02](https://github.com/Uniswap/v2-periphery/blob/master/contracts/UniswapV2Router02.sol)
  * [Curve Gauges](https://github.com/curvefi/curve-dao-contracts/blob/master/doc/README.md)

### Week 3 - 4: <a href="#week-3-4-wb-9th-may" id="week-3-4-wb-9th-may"></a>

Project: Smart contract challenge

### Week 5 - 4: <a href="#week-5-4-wb-23rd-may" id="week-5-4-wb-23rd-may"></a>

* Intro to the protocol/team or work idea
* Analyze main apps and branches from the project
* Produce dev documentation explaining how it works

### Week 6 - 8:  <a href="#week-6-8-wb-30th-may" id="week-6-8-wb-30th-may"></a>

* Working on the project. Specifics TBD and will be decided closer to the date

## Smart Contract Dev Study <a href="#smart-contract-dev-study" id="smart-contract-dev-study"></a>

Below is a curated list of resources that do an excellent job of explaining topics related to smart contract development. These should provide good foundational knowledge and hopefully help you identify additional subjects you may want to look into deeper. Also, if there is anything you think should be added, please feel free to add it.

**Cryptography**

* Public key cryptography
* Hashing functions
* Digital signatures
* [Mastering Ethereum - Chapter 4](https://github.com/ethereumbook/ethereumbook/blob/develop/04keys-addresses.asciidoc)

**Ethereum Virtual Machine & Gas**

* [Gas explained](https://ethgas.io/)
* [Intro to the EVM](https://ethereum.org/en/developers/docs/evm/)
* [EVM, Opcodes & Playground](https://www.evm.codes/) - Good for seeing how gas is calculated
* [EVM Puzzles](https://github.com/fvictorio/evm-puzzles)
* [Mastering Ethereum - Chapter 13](https://github.com/ethereumbook/ethereumbook/blob/develop/13evm.asciidoc)

**Solidity**

* [Official Solidity Docs](https://docs.soliditylang.org/en/latest/) - The best resource for learning solidity. Take your time studying the content.
* [Solidity by example](https://solidity-by-example.org/)
* [Solidity patterns](https://fravoll.github.io/solidity-patterns/)

**Secure Development**

* [Secureum - Security Pitfalls & Best Practices 101](https://secureum.substack.com/p/security-pitfalls-and-best-practices-101?s=r)
  * [Video](https://www.youtube.com/playlist?list=PLYORQHvGMg-XLdPc9Do8dWnjqtFcaDWEG)
* [Secureum - Security Pitfalls & Best Practices 201](https://secureum.substack.com/p/security-pitfalls-and-best-practices-201?s=r)
  * [Video](https://www.youtube.com/playlist?list=PLYORQHvGMg-Urml835vJRec\_hbPJYIb33)
* [Consensys Security Best Practices](https://consensys.github.io/smart-contract-best-practices/)
* [Trail of Bits Security Best Practices](https://github.com/crytic/building-secure-contracts)
* [Not So Smart Contracts](https://github.com/crytic/not-so-smart-contracts)

**Fun Stuff**

* [Ethernaut Solidity Trivia](https://github.com/ajsantander/trivias)
* [Smart contract wargames & writeups](https://github.com/blockthreat/blocksec-ctfs) - Start with Ethernaut
