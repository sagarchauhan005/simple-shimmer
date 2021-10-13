# Simple Shimmer

A simple, pure css shimmer for Vue, React, Angular or simple HTML. It acts as your pre-loader and is immensely beneficial to solve for PageSpeed issues.

# Screenshot

### Example
![Imgur](https://i.imgur.com/V4hiQSi.jpg)

### Code
![Imgur](https://i.imgur.com/rRXLRuf.jpg)

# Installation

Run `npm install @sagarchauhan005/simple-shimmer` into your app and then follow the steps.

# Usage

```
<script>

import SimpleShimmer from '@/simple-shimmer.vue';

export default defineComponent({
  components: {
    SimpleShimmer
  }
});

</script>

<template>
  <div id="app">
    <simple-shimmer :style="{height:'10px', width:'auto', borderRadius:'8px'}"/>
    <simple-shimmer :style="{height:'100px', width:'100px', borderRadius:'100%'}"/>
  </div>
</template>
```

- You can pass style tag inside the `:style="{}"` property and it will work out of the box.

# Author

[Sagar Chauhan](https://twitter.com/sagarchauhan005) works as a Project Manager - Technology at [Greenhonchos](https://www.greenhonchos.com).
In his spare time, he hunts bug as a Bug Bounty Hunter.
Follow him at [Instagram](https://www.instagram.com/chauhansahab005/), [Twitter](https://twitter.com/chauhansahab005),  [Facebook](https://facebook.com/sagar.chauhan3),
[Github](https://github.com/sagarchauhan005)

# License
MIT
