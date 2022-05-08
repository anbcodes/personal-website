# My personal website

I decided to write my personal website in raw html - hopefully it makes it last
longer with less maintenance.

Script to extract posts from my old website

```ts
console.log(
  "<li>\n" +
    projects.filter((v) => v.year === "2017").map((v) =>
      `${v.link ? `  <a href="${v.link}">\n  ` : ""}  ${v.name}${
        v.link ? `</a>` : ""
      }\n  - ${v.description}${
        v.codeLink ? ` -\n  <a href="${v.codeLink}">Github</a>` : ""
      }`
    ).join("\n</li>\n<li>\n") + "\n</li>",
);
```
