## Paste this code in browser console to make a file github URL to publicly accessible CDN

```js
const githubUrl =
  //Contents Github link here
  "https://github.com/user/repo/blob/main/image.png";

const raw = githubUrl
  .replace("https://github.com/", "https://raw.githubusercontent.com/")
  .replace("/blob/", "/");

console.log(raw);

const cdn = githubUrl
  .replace("https://github.com/", "https://cdn.jsdelivr.net/gh/")
  .replace("/blob/", "@");

console.log(cdn);
```
