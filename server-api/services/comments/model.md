# Model Comments

##Schema

```js
{
    userId: { type: String, required: true },
    contributionId: { type: String, required: true },
    content: { type: String, required: true },
    // Generated from content
    contentExcerpt: { type: String, required: true },
    upvotes: { type: Array, default: [] },
    upvoteCount: { type: Number, default: 0 },
    language: { type: String, required: true },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now },
    wasSeeded: { type: Boolean }
}
```