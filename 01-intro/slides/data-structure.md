# What is the data structure of blockchain?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

You can think of blockchain as a linked list of blocks. Each block contains a hash of the previous block, a timestamp, and transaction data. By making each block point to the previous one, you are forming a chain. This makes it extremely difficult to modify a past block, because doing so would require changing all subsequent blocks.

</div>
  <div>
    <img border="rounded" src="/linked-list.png">
  </div>
</div>
