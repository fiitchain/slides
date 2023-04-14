# Friends with Benefits

<div grid="~ cols-2 gap-2" m="t-2">
<div>

- A **peer** is comparable to full-node in Ethereum or Bitcoin. It maintains the state of the ledger, executes transactions and have multiple roles in the network.

- **Committing peer**
Maintains the state of the Blockchain and commits transactions. It verifies endorsements and validate the results of a transaction.

- **Endorsing peer**
An endorsing peer is always also a committing peer. The difference is that an endorsing peer  additionally takes transaction proposals and executes them to create endorsements.

-  The **number of peers in a network is not limited** and depends on the operating consortium.

- Chaincode supports the **emission of events**, e.g. when a certain transaction happened. Peers are  responsible for handling and delivering such events to subscribers (applications), publish /  subscribe architecture pattern.


</div>
  <div>
    <img border="rounded" src="/best-friends-anime-gif.gif">
  </div>
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>