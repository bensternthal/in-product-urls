# Test that Accept-Language header respects the order and weight of the requested locales


## First supported language check
```shell
curl -H "Accept-Language: xx,de" https://support.mozilla.org/kb/about-tiles-new-tab 
```

must return German (de)

## Order check
```shell
curl -H "Accept-Language: fr,de" https://support.mozilla.org/kb/about-tiles-new-tab 
```

must return French (fr)


## Weight check

```shell
curl -H "Accept-Language: fr;q=0.5,de" https://support.mozilla.org/kb/about-tiles-new-tab 
```

must return German (de)

