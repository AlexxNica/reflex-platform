### -dynamic flag on macOS

When invoking ghc directly on macOS, you'll need to give it `-dynamic` - otherwise, you will get something like

```
Undefined symbols for architecture x86_64:
  "_OBJC_CLASS_$_NSURL", referenced from:
      objc-class-ref in libHSjsaddle-wkwebview-0.9.4.0-2SHufpCZa9lIA8lareALCO.a(WKWebView.o)
ld: symbol(s) not found for architecture x86_64
```
