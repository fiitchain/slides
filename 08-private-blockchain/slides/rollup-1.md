# Should I be Optimistic about rollup?

> Rollups bundle (or ’roll up’) many transactions into a single transaction on layer 1.

<div grid="~ cols-2 gap-2" m="t-2">
<div>

- Optimistic rollups are 'optimistic' in the sense that transactions are assumed to be valid, but can be challenged if necessary. If an invalid transaction is suspected, a fraud proof is submitted and resolved onchain.
- On Ethereum, these are posted to a so called "calldata" and in the future to the blob storage provided by Danksharding.
- Validators must provide a bond before producing blocks.
- Rollup validators validate the blocks using their copy of the rollup state.
- If transition invalid, they can submit a fraud proof.

</div>
<div>
  <img border="rounded" src="/rollup-batch.svg">

  <img border="rounded" src="/fraud-proof.svg">

</div>
  
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>