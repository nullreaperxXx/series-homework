# series-homework

JavaScript functions for the SeriesHub site: reading JSON data, array functions,
updates without changing the original data, and fixing 3 bugs.

## How to run the check

```
node check.js
```

## Questions

**1. In addEpisode, why isn't `{ ...show }` enough? What did I create anew?**

I created new copies of: the series array, the show object, the seasons array, the season and the episodes array.
`{ ...show }` only copies the top level, so the seasons inside are still the same objects as the original.
That's why I had to copy every level on the way to the episode I change.

**2. In bug #3 the teammate used `...`. Why didn't it help?**

He used `push` on the original season before he made the copy.
Also, `{ ...show }` is a shallow copy, so the copy still shares the seasons array with the original.
So the episode was added to the original show too.