# Test that not translated articles fallback as specified in SOW.



## Verify The Following fallback

### Translated Falback Exists

```
https://support.mozilla.org/kb/flash-protected-mode-settings
an	es
ca	es
ca-valencia	es
csb	pl 
be	ru
br	fr
```

### No translation exists so fallback is just UX

```
https://support.mozilla.org/kb/certificate-pinning-reports
an	es
ca	es
ca-valencia	es
csb	pl
be	ru
br	fr
```

## Sanity Check The Following Fallbacks

```
de-at	de
de-ch	de
de-de	de
an	es 
ca	es
ca-valencia	es
es-ar	es
es-cl	es
es-es	es
es-mx	es
br	fr
oc	fr
gu	gu-in
hi	hi-in
lij	it
ja-jp-mac	ja
csb	pl
pt-br	pt-br
pt-pt	pt-br
be	ru
sv-se	se
sr-cyrl	sr
sr-latn	sr
ta-lk	ta
ta-in	ta-lk
ts	th

All others default to english
```
