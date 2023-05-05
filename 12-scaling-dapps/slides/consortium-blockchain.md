# And how do we get data from the dApp?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

- Usually via RPC (Remote Procedure Call) to the blockchain node.

- The access to the RPC node is limited and therefore we have a node providers (Infura, Alchemy)

- Once we are connected using `ethers.js` we can call the functions of the smart contracts.

- **Pros**:
  - Easy to use
  - Do not rely on any third party



</div>

  <div>
    <img border="rounded" src="/blushing-embarrassed.gif">
  </div>

  - **Cons**:
    - Not scalable (very slow)
    - No historical data
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>