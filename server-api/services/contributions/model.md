# Model

## Schema

```javascript
{
    userId: { type: String, required: true },
    categoryIds: { type: Array },
    title: { type: String, required: true },
    slug: { type: String, required: true, unique: true }, // Generated from title
    type: { type: String, required: true },
    content: { type: String, required: true },
    contentExcerpt: { type: String, required: true }, // Generated from content
    teaserImg: { type: String },
    language: { type: String, required: true },
    visibility: {
      type: String,
      enum: ['public', 'friends', 'private'],
      default: 'public'
    },
    emotions: { type: Object }
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now }
}
```

