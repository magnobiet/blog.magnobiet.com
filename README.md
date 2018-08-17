# blog.magnobiet.com

> Made with ♥ using [Jekyll](http://jekyllrb.com/).

Proudly hosted by [GitHub](https://github.com/).

[![CloudFlare](https://www.cloudflare.com/media/images/web-badges/cf-web-badges-c-gray-on.png)](https://www.cloudflare.com/)

## TL;DR

```bash
gem install bundler jekyll

jekyll new blog && cd $_
bundle install
jekyll serve --host=0.0.0.0

echo "blog.magnobiet.com" > CNAME

git init
git checkout -b gh-pages
git add .
git commit -m "Initial commit"
git remote add origin https://github.com/magnobiet/blog.git
git push -u origin gh-pages
```

## DNS record

```ini
;; CNAME Records
blog.magnobiet.com.	300	IN	CNAME	magnobiet.github.io.
```

## References

- https://jekyllrb.com/docs/home/
- https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/

## Licence

[MIT](https://magno.mit-license.org/2018)
