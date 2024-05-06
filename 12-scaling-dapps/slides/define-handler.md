# Define handler 📦💻


```ts
export async function handleTokenTransfer(context: Context): Promise<void> {
  const event = unwrap(context, getTransferTokenEvent);

  const id = createTokenId(event.collectionId, event.sn);
  const entity = await getWith(context.store, NE, id, { collection: true });

  entity.currentOwner = event.to;
  entity.updatedAt = event.timestamp;

  success(OPERATION, `${id} from ${event.caller} to ${event.to}`);
  await context.store.save(entity);
}
```

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>