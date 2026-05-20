Run this commain in browser console to convert image's github link to cdn link:

const githubUrl =
  "https://github.com/jasimbdpro/github-as-a-cdn/blob/main/uploads/09062d0b-f548-44ff-9844-4b4a0bfc75b3.jpg";

const raw = githubUrl
  .replace("https://github.com/", "https://raw.githubusercontent.com/")
  .replace("/blob/", "/");

console.log(raw);
