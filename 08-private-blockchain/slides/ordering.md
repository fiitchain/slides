# May I take your order?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

- **The ordering service** consists of one or more ordering nodes. The nodes do not store any  chaincode, nor do they hold the ledger.

- Eforces the network policy and takes care of the authentication and  authorization of the peers.

- Applications must submit transactions to an ordering service node. The node then collects  transactions and orders them sequentially. The transactions are then put into a new block and  delivered to all peers of a specific channel.

- The blocks are then broadcasted to the peers that hold the chaincode and the ledger. Before the transactions are committed, the peers validate it.


</div>
  <div>
    <img border="rounded" src="/big-smoke.gif">
  
  - Consensus is reached when the endorsement of a transaction is accepted, the ordering was  successful and the execution was valid and committed.
  </div>
</div>