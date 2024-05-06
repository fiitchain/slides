# Generate Typescript Classes and Chain types 🦑

<div grid="~ cols-2 gap-2" m="t-2">
<div>


- The squid processor data handlers use TypeORM entities 

- Therefore we do not need to write raw SQL queries

- **Only** indexer solution we can generate classes for on-chain data


```ts
export type TransferEvent = {from: string, to: string, tokenId: ethers.BigNumber}

export function decode721Transfer(ctx: Context): TransferEvent {
  const log = getEvmLog(ctx, ctx.event)
  return erc721.events["Transfer(address,address,uint256)"].decode(log)
}
```

</div>
  <div>
    <img border="rounded" src="/cat-sewing.gif">
  </div>
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>