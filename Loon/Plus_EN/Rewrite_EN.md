# Copy

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) When receiving an http request, Loon will use the requested url to find a matching url rewrite, and a URL Rewrite will match Replace or modify the url in the HTTP request, or replace the request response body.

## format requirement

![#f03c15](https://placehold.it/15/f03c15/000000?text=+) A URL Rewrite is divided into three parts: regular expression, replacement content, rewrite type

### E.g

```
https?://(www.)?g.cn https://www.google.com 302
```

## Support type

-header

   -The matching host field in the request header will be replaced by the replacement content

-reject

   -Directly reject the request

-302
  
   -Return 302 response

-307

   -Return 307 response

# Reference

-[LoonManual](https://github.com/Loon0x00/LoonManual/blob/master/README.md)