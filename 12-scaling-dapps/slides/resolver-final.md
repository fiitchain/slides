# A time for resolver (3)

touch resolvers/nftEvents.ts

Third, we finish the resolver:

```ts
@Resolver()
export class NFTEventResolver {
  constructor(private tx: () => Promise<EntityManager>) {}

  @Query(() => [TokenEventEntity])
  async nftEventListByType(
    @Arg('type', { nullable: false }) type: Interaction,
    @Arg('limit', { nullable: true, defaultValue: null }) limit: number,
  ): Promise<TokenEventEntity[]> {
    const result: TokenEventEntity[] = await makeQuery(this.tx, EventEntity, nftEventList, [type, limit])
    return result
  }
}
```

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>