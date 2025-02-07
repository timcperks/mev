# 🏴‍☠️ mev on ethereum

<br>


### in this repo

<br>

* [basic evm](evm-knowledge.md)
* [eip-1559](eip-1559.md)
* [the mempool](MEMPOOL.md)
* [terminology](terminology.md)



<br>


<img width="900" alt="Screen Shot 2022-11-17 at 2 02 06 PM" src="https://user-images.githubusercontent.com/1130416/202569415-5b0b7eff-5fe9-4c83-8249-702822d0766d.png">



<br>

<img width="400" alt="Screen Shot 2022-10-17 at 10 19 34 PM" src="https://user-images.githubusercontent.com/1130416/196341991-97ef37f7-c509-448f-a08c-95043fbe4fef.png">






<br>

----

### terminology




* **Block builder**
The agent responsible for assembling the potential contents of a block (i.e. the set of transactions that makes up the “payload” of a block). In Proof of Work Ethereum it’s the miner. In Proof of Stake Ethereum it’s the validator, but this activity can separated from the validator via PBS, in which case builders need to submit bids for blocks to be included to the block proposer for inclusion.

* **Block proposer**
The agent responsible for proposing new blocks in a blockchain. In Proof of Work Ethereum it’s the miner. In Proof of Stake Ethereum it’s the validator.

* **Node Operator**
An organization/entity/person that operates validators.

* **PBS**
Proposer Builder Separation, see: State of research: increasing censorship resistance of transactions under proposer/builder separation (PBS).

* **Staker**: A user/organization/etc. which holds (w)stETH

* `feeRecipient`: field set by the block builder in the block header (coinbase address)

* payment methods on Ethereum:
   - `base_fee`: amount defined by the protocol, always paid from user -> network
   - `priority_fee`: amount defined by the user as `maxPriorityFeePerGas`, paid from user -> coinbase address
   - `block.coinbase transfer`: the EVM has an opcode which allows end user to send fund directly to the coinbase address (same recipient as `priority_fee`
    - `regular transfer`: a transaction created to send eth to other account
    
    
 <br>
 
 ---
 
 ### resources
 
 * [mev on eth2 talk by vitalik](https://www.youtube.com/watch?v=OD54WfVuDWw&list=PLRHMe0bxkuel3w3C7P_WVvp9ShLi3HKRI&index=30)
 * [updates on pbs video by barnabe monnot](https://archive.devcon.org/archive/watch/6/updates-on-proposer-builder-separation/?tab=YouTube)
