# Model

## Schema

```javascript
{
    image: imageSchema,
    // may be temporary or some other status
    status: { 
      type: String, 
      enum: ['permanent', 'temporary'], 
      default: 'permanent',
      required: true
    }, 
    // the type off the badge, e.g.
    // Crowdfounder badge is a one time forever badge
    // some badges are given got by an achivement
    // some badges given by events or they are a gift form an other user
    // some badges may be temporary like moderator badge
    type: { type: String, required: true },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now }
}
```

