# Model

## Schema

```javascript
{
    userId: { type: String, required: true },
    contributionId: { type: String, required: true },
    rated: {
      type: String,
      required: true,
      enum: ['funny', 'happy', 'surprised', 'cry', 'angry']
    },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now },
    wasSeeded: { type: Boolean }
}
```

