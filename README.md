# context-example

# Start

```
ns run ios
```

# Test
1. Click on the increment button
2. Click on the `Navigate to next page` button
3. See that context is no longer accessible fails with:
  ```
***** Fatal JavaScript exception - application has been terminated. *****
  NativeScript encountered a fatal error: Uncaught TypeError: Cannot destructure property 'testInformation' of '(0 , svelte_internal__WEBPACK_IMPORTED_MODULE_0__.getContext)(...)' as it is undefined.
  ```
