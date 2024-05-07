# Can we see the difference on the code?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

```js
const { ethers } = require('ethers');
const contractAddress = 'INSERT_CONTRACT_ADDRESS_HERE';
const abi = [INSERT_CONTRACT_ABI_HERE];

async function getFirst10NFTs() {
  const provider = new ethers.providers.JsonRpcProvider();
  const contract = new ethers.Contract(contractAddress, abi, provider);

  const totalSupply = await contract.totalSupply();
  const nfts = [];

  for (let i = 0; i < Math.min(totalSupply, 10); i++) {
    const nftId = await contract.tokenByIndex(i);
    const nft = await contract.getNFT(nftId);
    nfts.push(nft);
  }

  return nfts;
}

getFirst10NFTs().then(console.log).catch(console.error);
```

</div>
  <div>

  ```graphql
    query getFirst10NFTs($id: String!) {
      nftEntities(limit: 10, where: {collection: {id_eq: $id}}) {
        id
        name
        metadata
      }
    }
  ```


  </div>
</div>

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>