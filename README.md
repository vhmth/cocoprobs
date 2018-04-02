According to [Starscream's docs](https://github.com/daltoniam/Starscream#add-copy-frameworks-phase) we want to add Starscream
in both "Link Binary with Libraries" as well as "Copy Frameworks" (a "Copy Files" Build Phase that sets the destination to
"Frameworks"). When I do the second step, I get the following error:

```
Unable to run command 'PBXCp Starscream.framework' - this target might include its own product.
```

# Setup

1. `cd test && pod install`
2. `open test/test.xcworkspace`
3. `cmd + B` to build
