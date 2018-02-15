# ShareIQ local homebrew packages

## Enable:

```shell
brew tap shareiq/local
brew tap-pin shareiq/local
```

## Disable:

```shell
brew untap shareiq/local
```

# List of Packages:

## Opencv

Same as core, but with added jpeg2000 support

```shell
brew install opencv
```

# Build instructions:

Note to self:

```
brew uninstall opencv
brew install --build-bottle ./opencv.rb
brew bottle opencv
gsutil cp opencv-3.4.0_1.high_sierra.bottle.1.tar.gz gs://shareiq-packages/brew/
```

If the package is aleady installed, use `upgrade` instead of `install`.
