# Snapshot data of valuable Web3 users [DEPRECATED]


## Dataset Overview

As web3 technology rapidly advances, the industry is bustling with transformative potential. However, the growth has been tainted by disruptors exploiting the technology: sybil addresses, airdrop hunters, bot addresses with low net worth are everywhere on the chain. 

The lack of precise, comprehensive, and public datasets of high-quality on-chain users hampers developers or researchers from effectively identifying the authenticity and value of on-chain users. This creates roadblocks in building better user solutions and conducting industry-related academic analyses. 

DeBank, as a leading user platform in the web3 industry, we're working actively to address these challenges. Our proficiency in user portfolios, quality definition, and computational analysis makes us an authoritative voice. From time to time, we'll share snapshots of our foundational dataset used to solve these problems with the community for free to move the industry forward.

## Dataset Content

[Dataset](./valuable-users) includes users meeting any of the below requirements:
- Net worth > 1000USD
- "Web3 ID" minted
- Addresses have followers on DeBank and TVF>0

## Parameters

- addr（string）
  > 0x address, only supports address on EVM compatible chains
- usd_value(double)
  > net worth (USD) of the address, only supports address >1000 USD
- web3_id（string） 
  > The Web3 identity minted by this address and used to be recognized in the community. It's binded to this address, not changeable nor transferrable.
- follower_count（int）
  > Number of its followers on DeBank
- tvf（double)
  > "Total Value of Followers": the sum of all its DeBank followers' net worth (USD)

## Data Structure

```
[
    {
       // 0x address, only supports address on EVM compatible chains
        "id": "0x5853ed4f26a3fcea565b3fbc698bb19cdf6d0000", 
        // net worth (USD) of the address, only supports address >1000 USD
        "usd_value": 5763.151883,  
        // the unique "Web3 ID" binded to this address
        "web3_id": "tester", 
        // number of its followers on DeBank
        "follower_count": 12368, 
        // "Total Value of DeBank Followers"(USD)
        "tvf": 74669506.257037 
    }
]
```

## Data Scope
Data includes up to 57 mainstream EVM compatible chains since its initial release.

Data sources include public data information from addresses behavior on EVM-compatible chains and from the DeBank platform.

## Usage & Updates

The [dataset](./valuable-users) is currently available for callers to use for free.

Our engineers will manually update the snapshots from time to time. You can subscribe for updates if needed.

If you need on-chain users' real time data, you can visit DeBank Cloud to use the paid Open API service here:
https://docs.cloud.debank.com/en/readme/api-pro-reference/user

Feel free to contact us at:hello.cloud@debank.com
  
  

