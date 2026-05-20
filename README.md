### Paste this code in browser console to make a file's github URL to publicly accessible CDN URL (every image/file's name should include unique id like "_Uid_N3Te" at last):

```js
const githubUrl =
  //Content's Github URL here
  "https://github.com/user/repo/blob/main/image_Uid_N3Te.png";

const raw = githubUrl
  .replace("https://github.com/", "https://raw.githubusercontent.com/")
  .replace("/blob/", "/");

console.log(raw);

const cdn = githubUrl
  .replace("https://github.com/", "https://cdn.jsdelivr.net/gh/")
  .replace("/blob/", "@");

console.log(cdn);
```
