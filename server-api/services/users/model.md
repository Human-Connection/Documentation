# Model

## Schema

```javascript
{
    email: {type: String, required: true, unique: true},
    password: { type: String },
    name: { type: String },
    slug: { type: String },
    gender: { type: String },
    followerIds: [],
    follows: [followsSchema],
    isnothere: { type: Boolean },
    timezone: { type: String },
    avatar: { type: String },
    coverImg: { type: String },
    doiToken: { type: String },
    confirmedAt: { type: Date },
    badgeIds: [],
    deletedAt: { type: Date },
    createdAt: { type: Date, default: Date.now },
    updatedAt: { type: Date, default: Date.now },
    // Needed for verification
    isVerified: { type: Boolean },
    role: {
      type: String,
      enum: ['admin', 'moderator', 'manager', 'editor', 'user'],
      default: 'user'
    },
    verifyToken: { type: String },
    verifyShortToken: { type: String },
    verifyExpires: { type: Date },
    verifyChanges: { type: Object },
    resetToken: { type: String },
    resetShortToken: { type: String },
    resetExpires: { type: Date },
    wasSeeded: { type: Boolean },
    wasInvited: { type: Boolean },
    language: { type: String, default: 'en' }
}
```

