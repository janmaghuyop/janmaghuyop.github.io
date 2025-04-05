#
## Links
- https://css-tricks.com/emoji-as-a-favicon/
## Minify
```bash
cd ~/bin
# https://github.com/wilsonzlin/minify-html
VERSION=0.16.4
wget https://github.com/wilsonzlin/minify-html/releases/download/v$VERSION/minhtml-${VERSION}-aarch64-apple-darwin
mv minhtml-$VERSION-aarch64-apple-darwin minhtml
minhtml --output index.html --minify-css --minify-js main.html
# reduce pic size
convert selfie.jpg -quality 80 -strip -define webp:lossless=false -define webp:method=6 output.webp
convert selfie.jpg -quality 5 -strip -define webp:lossless=false -define webp:method=6 output.webp
```
