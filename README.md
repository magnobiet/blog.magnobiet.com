# [Magno’s Blog](https://blog.magnobiet.com/)

> Made with ♥ using [Jekyll](http://jekyllrb.com/) and proudly hosted by [GitHub](https://github.com/).

[![CloudFlare](https://www.cloudflare.com/media/images/web-badges/cf-web-badges-c-gray-on.png)](https://www.cloudflare.com/)

## TL;DR

```bash
# install jekyll
gem install bundler jekyll

# create a new jekyll project
jekyll new blog && cd $_
```

### Development

```bash
npm install

# run development environment
npm run start

# run jekyll build
npm run build
```

## DNS

```ini
;; CNAME Records
blog.magnobiet.com.	300	IN	CNAME	magnobiet.github.io.
```

### CNAME

```bash
echo "blog.magnobiet.com" > CNAME
```

## References

- https://jekyllrb.com/docs/home/
- https://jekyll.github.io/jekyll-admin/
- https://github.com/jekyll/minima
- https://help.github.com/articles/setting-up-your-github-pages-site-locally-with-jekyll/
- https://carlosbecker.com/posts/jekyll-reading-time-without-plugins/

## License

This project is licensed under the [MIT License](https://magno.mit-license.org/2018-2021). Copyright © Magno Biét
