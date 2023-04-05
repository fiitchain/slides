# What is the data structure of blockchain?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

- **linked list of blocks**

- each block contains: a hash of the previous block, a timestamp, and transaction data. 

- By making each block point to the previous one, you are forming a chain.

- extremely difficult to modify a past block, because doing so would require changing all subsequent blocks.

</div>
  <div>
    <img border="rounded" src="/linked-list.png">
  </div>
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>