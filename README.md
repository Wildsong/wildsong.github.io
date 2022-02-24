# wildsong.github.io

Home page for the Wildsong organization

It will show up on https://wildsong.github.io/
and https://www.wildsong.biz/


## Testing and development

This command will run a Jekyll server.
See http://localhost:4000/

Create boilerplate (for new projects only)

```bash
export REPO="$USERPROFILE/source/repos/wildsong.github.io"
docker run --rm --name=jekyll --volume="$REPO:/srv/jekyll" jekyll/jekyll jekyll new website
```

Run a test server, with hot reload

```bash
export REPO="$USERPROFILE/source/repos/wildsong.github.io"
docker run --rm --name=jekyll \
  --volume="$REPO:/srv/jekyll" \
  --publish 4000:4000 \
  jekyll/jekyll \
  jekyll serve --incremental
```

(Do I want --incremental?)
