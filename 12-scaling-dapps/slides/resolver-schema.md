# A time for resolver (2)

touch model/event.model.ts

Second, we have to create the model:

```ts
@ObjectType()
export class TokenEventEntity {
  @Field(() => String, { nullable: false })
  id!: string
  @Field(() => String, { nullable: true })
  name!: string
  @Field(() => Date, { nullable: false })
  date!: Date
  @Field(() => String, { nullable: true, defaultValue: '' })
  meta!: string
  @Field(() => String, { nullable: true, defaultValue: '' })
  image!: string
  @Field(() => String, { nullable: false })
  issuer!: string
  @Field(() => String,{ nullable: false })
  caller!: string
}
```

<div class="absolute right-5px bottom-5px">
<SlideCurrentNo /> / <SlidesTotal />
</div>