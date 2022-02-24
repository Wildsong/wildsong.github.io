# wildsong.github.io

Home page for the Wildsong organization

It will show up on https://wildsong.github.io/
and https://www.wildsong.biz/


## Testing and development

This command will run a Jekyll server.
See http://localhost:4000/

docker run --rm \
  --volume="$PWD:/srv/jekyll" \
  --publish [::1]:4000:4000 \
  jekyll/jekyll \
  jekyll serve

