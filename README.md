# Hyde

My personal blog.
Buld using (https://github.com/poole/hyde)

[Thanks to  Mark Otto.](https://github.com/mdo)

docker run --rm --volume="$PWD:/srv/jekyll" --volume="$PWD/vendor/bundle:/usr/local/bundle"  -it --name jblog -p 4000:4000 jekyll/jekyll:4.0 jekyll s