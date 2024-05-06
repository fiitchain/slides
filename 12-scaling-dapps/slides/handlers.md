# Define handlers for the app


- We want to tell processor which data we want to index

- We can filter by contract events, transactions

- Filter can be fine-tuned by the block number, address, topics

```ts
const CONTRACT_ADDRESS = '0x...'
const transferFilter: EvmLogHandlerOptions = {
  filter: [erc721.events["Transfer(address,address,uint256)"].topic],
}
processor.addEvmLogHandler(CONTRACT_ADDRESS, transferFilter, handleTokenTransfer);
```


<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>