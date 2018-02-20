# Contributions Service

The Contribution Service deals with posts, votes, etc.

> **Question:** Should votes, pro cons, etc. be split of form contributions?
>
> In tearms of searchability etc. it might be easier to only search one service that contains all types of contributions!?

## Schema

```js
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

## Interaction

* Comments
* Let's Talk
* Version

## More Info

List all Contributions and Chatrooms that match the current Contribution.

_The matching happens by Categories and Tags._

* Posts
* Can Do's
* Bestlists
* Pro / Cons
* Votes
* Chatrooms

## Take Action

* Projects
* Can Do's
* Projects
* Jobs
* Events
* Map



