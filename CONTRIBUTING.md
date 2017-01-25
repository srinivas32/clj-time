# Contribution Guidelines for clj-time

## Generating Documentation

We generate documentation using codox.

From the `master` branch, run

```bash
lein doc
cp -R doc{,.new}
git checkout gh-pages
rm -rfv doc
mv -v doc{.new,}
```

Then add the new contents and issue a PR against `gh-pages` from your
fork.
