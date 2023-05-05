# How does the processing works?

<div grid="~ cols-2 gap-2" m="t-2">
<div>

1. For each block, extracts all requested transactions/events.
2. For each event/transaction, call the pre-defined handler.
3. Handler should transform the data to match the schema we defined.
4. Save into the Postgres database.


</div>
  <div>
    <img border="rounded" src="/you-just-got-to-draw-draw-with-your-mouth.gif">
  </div>
</div>

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>