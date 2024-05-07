# Model the data with a schema

<div grid="~ cols-2 gap-2" m="t-2">
<div>

```graphql
type CollectionEntity @entity {
  blockNumber: BigInt
  createdAt: DateTime!
  currentOwner: String
  id: ID!
  issuer: String
  max: Int!
  meta: MetadataEntity
  metadata: String
  name: String
  nfts: [NFTEntity!] @derivedFrom(field: "collection")
  symbol: String
  version: String
}
```


</div>
  <div>
    <img border="rounded" src="/ellenoar-seiran.gif">
  </div>
</div>

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>