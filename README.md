# series-homework

JavaScript functions for the SeriesHub site: reading JSON data, array functions,
updates without changing the original data, and fixing 3 bugs.

## How to run the check

```
node check.js
```

## Questions

**1. In addEpisode, why isn't `{ ...show }` enough? What did I create anew?**

I created new copies of: the series array, ______, ______, ______ and ______.
`{ ...show }` only copies ______, so the seasons inside are still ______.
That's why I had to copy every level on the way to ______.

**2. In bug #3 the teammate used `...`. Why didn't it help?**

He used `push` on ______ before ______.
Also, `{ ...show }` is a shallow copy, so the copy still shares ______ with the original.
So the episode was added to ______ too.