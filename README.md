# Essays

Personal essays site — [rmatte01.github.io/essays](https://rmatte01.github.io/essays)

## Posting a new essay

```bash
cp _essays/_template.md _essays/YYYY-MM-DD-your-title.md
# edit the file
git add . && git commit -m "essay: your title" && git push
```

Live in ~60 seconds.

## Local preview

```bash
gem install bundler
bundle install
bundle exec jekyll serve
# → http://localhost:4000/essays/
```
