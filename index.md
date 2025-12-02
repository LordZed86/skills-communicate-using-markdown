# H1 Test

## Image

![IMG_2256](https://github.com/user-attachments/assets/0c9eed4e-baca-49fc-b3a7-2bbaff7d706c "A king charles cavalier dog laying in a red bed")

## code example

```JavaScript
function reviewFilesFor(bookFolder) {
  const dir = path.join(BOOKS_DIR, bookFolder);
  const files = fs.readdirSync(dir);
  return files
    .filter((f) => /^review\d+\.txt$|^review\d{2}\.txt$/i.test(f)) // regex match
    .sort((a, b) => a.localeCompare(b)) // ensure stable order (alphabetical)
    .map((f) => path.join(dir, f)); // return full paths
}
```
## Task List

- [x] Github intro
- [ ] Markdowm intro
- [ ] pull request review
- [ ] merge conflicts
