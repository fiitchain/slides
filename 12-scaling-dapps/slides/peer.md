# A time for resolver (1)

<div grid="~ cols-2 gap-2" m="t-2">
<div>

```sql
SELECT e.meta, e.timestamp as date, ne.id, ne.name, me.image, ne.issuer, e.caller
FROM event e
LEFT JOIN nft_entity ne ON ne.id = e.nft_id
LEFT JOIN metadata_entity me ON me.id = ne.meta_id
WHERE e.interaction = $1
ORDER BY e.timestamp DESC
LIMIT $2
```

</div>
  <div>
    <img border="rounded" src="/best-friends-anime-gif.gif">
  </div>
</div>
<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>