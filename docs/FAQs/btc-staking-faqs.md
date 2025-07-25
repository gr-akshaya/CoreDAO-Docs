---
sidebar_label: Self-Custodial BTC Staking FAQs
hide_table_of_contents: false
sidebar_position: 2
---

# Self-Custodial Bitcoin Staking FAQs
---

### 1. What is Self-Custodial Bitcoin Staking on the Core network?

Core provides Bitcoin holders with a risk-free and transparent opportunity to lock up or stake their Bitcoin on the Bitcoin Network without relinquishing custody of their Bitcoin assets. In return, they can participate in the Core blockchain’s security through Satoshi Plus and earn CORE rewards.

### 2. How does Self-Custodial Bitcoin Staking work?

With Self-Custodial Bitcoin Staking, Core's protocol incorporates bitcoin holders into its consensus mechanism, Satoshi Plus. Core's methodology for integrating Bitcoin staking centers on [CLTV timelock](https://en.bitcoin.it/wiki/Timelock#CheckLockTimeVerify), a Bitcoin-native cryptographic feature that specifies a condition under which the transaction output cannot be spent until a particular point in time has passed. For more details on how Self-Custodial Bitcoin Staking works, refer [here](../stake-and-delegate/btc-staking/btc-staking-working.md).

### 3. What are the advantages of Self-Custodial Bitcoin Staking?

1. **Tailored for Long-Term Holders and Institutions:** Designed for those who prefer to keep their bitcoins on the secure Bitcoin blockchain, Self-Custodial Bitcoin Staking offers a way to earn rewards during a specified holding period without requiring frequent transactions.  
2. **No New Trust Assumptions:** Users can stake their bitcoins directly on the Bitcoin blockchain, maintaining the high security and trust inherent in Bitcoin's robust infrastructure without transferring assets off-chain.  
3. **Opportunity to Earn Passive Rewards:** Bitcoin stakers can earn CORE token rewards in exchange for contributing to the Core blockchain's consensus, enhancing the blockchain's functionality and security.  
4. **Self-Custody and Security:** Bitcoin Staking is 100% secure with self-custody; users execute staking transactions themselves on the Bitcoin network, ensuring their Bitcoin remains on the blockchain.  
5. **Use of Native Cryptographic Features:** Bitcoin staking on Core utilizes battle-tested cryptographic features of the Bitcoin network, making it safer than non-native solutions.  
6. **Flexibility in Transaction Building:** Users can build their staking transactions using any preferred tool, significantly reducing the risk of supply chain attacks from third-party libraries.

### 4. How does Self-Custodial Bitcoin staking maintain security and trust?

Core's Self-Custodial Bitcoin staking eliminates the need to introduce new trust assumptions by enabling users to stake their bitcoins without transferring them off the Bitcoin blockchain. It leverages Bitcoin's established infrastructure's inherent security and trust, maintaining high security for staked assets.

### 5. What is the role of Core in the process of Self-Custodial Bitcoin staking?
It is noted here that no assets are moved onto the Core blockchain or into any trusted third-party or smart contracts. Instead, users' assets remain locked on the Bitcoin network under the complete ownership of the user. From the Core’s perspective, only the relayers monitor the Bitcoin network for any Bitcoin staking transactions. Upon detection, these are selected, and only the valid ones are passed down to the consensus engine for the accrual of staking rewards. With the Fusion Upgrade, users would have to manually claim their staking rewards in the form of CORE tokens.

### 6. What happens to my asset in the validator I delegated my Bitcoins to, or the Core blockchain goes down?

Delegating Bitcoins for staking rewards through Core’s Self-Custodial Bitcoin does not require any kind of asset transfers or bridging onto the Core blockchain or to validators. Even if the validators or the Core blockchain go down, users' assets remain in their complete custody and can be redeemed after the timelock expires on the Bitcoin network.

### 7. What are some challenges associated with Short Time Locks on Bitcoin?

CLTV timelock is a native feature of the Bitcoin network. A user can lock up any amount of Bitcoin for the desired period through this feature. However, with shorter time lock periods (e.g., 10 minutes) due to network congestion and Bitcoin network block times, these transactions may not be processed quickly enough, leading to delays in redeeming the Bitcoin. Note that for a Bitcoin staking transaction to be valid, the minimum requirements should be met.

### 8. Are there any specific requirements to participate in Self-Custodial Bitcoin Staking?

Users must meet the following requirements for a Bitcoin staking transaction to be considered valid.

* Users must ensure that the transaction is sent to their address.  
* Using the Bitcoin native timelock feature, specify the lock-up amount intended to be delegated to the validator on the Core blockchain as the transaction output.  
* When using the staking script, there is **no** minimum Bitcoin requirement for staking. However, if staking through the [official staking website UI](https://stake.coredao.org/staking), users must stake at least **0.01 BTC** (excluding transaction fees).
* Minimum staking duration depends on the method. The official website UI requires a 5-day minimum, while staking through the script has no lockup requirement.

* The transaction should also contain an `op_return` output specifying  
  * The address of the Core Validator the staker wants to delegate their Bitcoin to.  
  * The address to which the staker would like their CORE token rewards to be sent.

### 9. Why does the staking address provided differ from your original Bitcoin address?

The staking address is derived from your wallet's master private key, ensuring your control and security over your assets. Your Bitcoins remain safely stored in your original wallet, unaffected by the staking process. While staked assets may not be visible in some wallet versions, you still have complete ownership.

You can view your staked funds by searching for the staking address on any Bitcoin explorer, such as [Mempool](https://mempool.space/). We're actively working to make staked assets visible in all supported wallets, primarily through command-line versions.

### 10. Does Core provide hardware wallet support for Self-Custodial Bitcoin Staking?

Due to technical constraints, Self-Custodial Bitcoin Staking does not currently support hardware wallets. Nevertheless, we continually explore ways to enhance compatibility with various wallet types, prioritizing both security and convenience for our users.

### 11. What are the important considerations for Locking Periods before staking your assets?

* **Time Lock Expiration: **When you lock your Bitcoin for staking, it's inaccessible until the staking period concludes.  
* **Choosing wisely:** Select your locking period thoughtfully, considering your investment objectives and risk tolerance. Starting with shorter locking periods can help you become familiar with the process before committing to longer durations.  
* **Staked Amount Verification:** Due to technical complexities, it is possible that your staked asset may not be visible in your wallet when checked through the CLI. However, you can easily verify that you have complete ownership of your staked assets from the [Core's Official Staking Website](https://stake.coredao.org/). Additionally, delays due to block time, the number of block confirmation requirements, and network congestion on the Bitcoin network may lead to delays in transaction confirmation, making your assets not visible in your wallets.

### 12. Why is my staked asset not visible in my wallet?

Due to technical complexities, it is possible that your staked asset is not visible in your wallet when checked through the CLI. However, you can easily verify that you have complete ownership of your staked assets from the [Core's Official Staking Website](https://stake.coredao.org/). Additionally, delays due to block time, the number of block confirmation requirements, and network congestion on the Bitcoin network may lead to delays in transaction confirmation, making your assets not visible in your wallets.

### 13. How is the security of Self-Custodial Bitcoin Staking ensured?

[Halborn](https://www.halborn.com/), a SOC2 Type 1 compliant firm renowned for its smart contract security expertise and [trusted by leading blockchain platforms](https://www.halborn.com/about/who-trusts-us) like Ava Labs, Solana, and Polygon, as well as DeFi projects like Sushiswap, has thoroughly audited Core's protocol and Self-Custodial Bitcoin Staking's security. You can review audit reports on Core's protocol and Self-Custodial Bitcoin Staking by leading firms [here](https://docs.coredao.org/docs/Learn/audit).

### 14. What should you do if the *`Redeem BTC`* button is not working on the staking website?

You can Redeem your Bitcoin by clicking the `Redeem` button on Core's official [Staking Website](https://stake.coredao.org/). If the button is not working, try clearing your browser cache and re-try. If you encounter further issues, please reach out at [Core Dev Forum](https://forum.coredao.org/).