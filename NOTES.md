# Notes



## Tips

### relative_url

Always use `relative_url` e.g.:

```
"{{ '/' | relative_url }}"
```

instead of the "old way" with `site.path` / `site.baseurl`:

```
"{{ site.path }}/"
```



## Todo


Remove all `site.path` references with `relative_url` e.g.:

```
<img src="{{site.path}}/themes/thumbnails/{{theme.thumbnail}}">
```

to

```
<img src="{{ '/themes/thumbnails/' | relative_url }}{{theme.thumbnail}}">
```
