# Model Categories

##Schema

```js
{
    title: { type: String, required: true },
    // Generated from title
    slug: { type: String, required: true, unique: true },
    icon: { type: String, unique: true },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now }
}
```