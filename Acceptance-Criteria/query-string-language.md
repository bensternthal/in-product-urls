# Test that correct article is returned when language is specified as query parameter.

_Note lithium will need to provide name of query parameter XXX used as placholder._



## Test specifying locale.
```shell
https://support.mozilla.org/kb/about-tiles-new-tab?XXX=de
```

must return German (de)

## Test overriding locale in path.
```shell
https://support.mozilla.org/en-US/kb/about-tiles-new-tab?XXX=de
```

must return German (de)

## Test translation does not exist for locale specified but does for fallback.

```shell
https://support.mozilla.org/kb/flash-protected-mode-settings?xxx=an
```

must return spanish (es) 

## Test translation does not exist for locale specified & does not exist for fallback.

```shell
https://support.mozilla.org/kb/certificate-pinning-reports?xxx=an
```

must return english (en) 

