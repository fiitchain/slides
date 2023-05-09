# Holy trinity of blockchain indexing

<div grid="~ cols-3 gap-1" m="t-2">


<div>

- 🕸 **The Graph** - rubick
  - ~ 300 bps
  - EVM (L1), NEAR
  - no ability for external calls
  - *self-hosted*
  - no ability for custom queries
  
</div>

<div>

- 📝 **SubQuery** - magick
  - ~ 500 bps
  - EVM (L1), Substrate, Cosmos
  - ability for external calls (~ 2yrs since we asked for that, unstable)
  - aggregations out of the box
  - auto-balanced for more nodes
  - (back in dayes) backbone of KodaDot's RMRK markteplace
</div>

<div>

- 🦑 **SubSquid** - rubick
  - ~ 50 000 bps
  - EVM (L1+L2), Substrate
  - can be used for external calls (fetch metadata from IPFS)
  - can write custom queries through resolvers
  - real time indexing
  
</div>



</div>

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>