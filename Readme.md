# Simple Shimmer

A simple, pure css shimmer for your website. It acts as your pre-loader and is immensely beneficial to solve for PageSpeed issues.

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

# Nuxt - SSR Usage

To make sure this runs on server side, you need to create your build with the following command:
```
nuxt build --standalone
```

You can add the command in your `scripts` section in the package.json file like this : 

```
"scripts": {
    "build": "nuxt build --standalone",
  },
```

### Why is this needed?

* Nuxt doesn't build dependencies that are required on the server side. The default way to do so is to pass node_modules to the server side.
* Passing node_modules to the server side is not a good practice.
* Running the build command above will build the dependencies on the server side. The make it possible to bundle all the dependencies into the final artifact for the server side part.
* You can read more about it here:
  * https://stackoverflow.com/questions/50700680/nuxt-start-requires-node-modules-to-be-present-in-order-to-run
  * https://github.com/nuxt/nuxt.js/issues/4292

# Author

[Sagar Chauhan](https://twitter.com/sagarchauhan005) works as a Project Manager - Technology at [Greenhonchos](https://www.greenhonchos.com).
In his spare time, he hunts bug as a Bug Bounty Hunter.
Follow him at [Instagram](https://www.instagram.com/sagarchauhan005/), [Twitter](https://twitter.com/sagarchauhan005),  [Facebook](https://facebook.com/sagar.chauhan3),
[Github](https://github.com/sagarchauhan005)

# License
MIT
