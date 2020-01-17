# atyasu/wkhtmltoimage

Dockerized wkhtmltoimage from https://hub.docker.com/r/icalialabs/wkhtmltopdf

This use IPA-JP Font.

# Usage

```shell
# The example found at https://wkhtmltopdf.org:
docker run --rm -v $(pwd):/root atyasu/wkhtmltoimage-jp https://yahoo.co.jp/ yahoo.jpg
```

オプションもりもり

```shell
docker run -v $(pwd):/root atyasu/wkhtmltoimage-jp --width 1024 --custom-header "User-Agent" "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_2) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/79.0.3945.94 Safari/537.36" --enable-javascript --javascript-delay 1000 --quality 100 --format png https://yahoo.co.jp/ test.png
```

# References

## Similar projects:

- https://hub.docker.com/r/icalialabs/wkhtmltopdf
- https://gist.github.com/akihiromukae/288b163d538d45a197b3f1b54ef385e8

# License

MIT (c) a-yasui
