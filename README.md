HTTP RFCs For Kindle
====================

`ebook-convert`ed RFCs. Original document is here: http://httpwg.org/specs/

```sh
for rfc in rfc{7230..7235}; do
  curl http://httpwg.org/specs/${rfc}.html > ${rfc}.html
  ebook-convert $rfc.html ${rfc}.mobi
done
```
