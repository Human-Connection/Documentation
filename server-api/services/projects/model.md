# Model Projects

##Schema

```js
{
    name: { type: String, required: true },
    slug: { type: String },
    followerIds: [],
    categoryIds: { type: Array },
    logo: { type: String },
    userId: { type: String, required: true },
    description: { type: String, required: true },
    content: { type: String, required: true },
    addresses: { type: Array, default: [] },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now },
    wasSeeded: { type: Boolean }
}
```