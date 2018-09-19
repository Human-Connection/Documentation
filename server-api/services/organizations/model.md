# Model

## Schema

```javascript
{
    name: { type: String, required: true },
    slug: { type: String },
    followerIds: [],
    categoryIds: { type: Array },
    logo: { type: String },
    userId: { type: String, required: true },
    description: { type: String, required: true },
    addresses: { type: Array, default: [] },
    content: { type: String, required: true },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now },
    wasSeeded: { type: Boolean }
}
```

