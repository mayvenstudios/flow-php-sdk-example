# Flow PHP SDK

> :warning: This is an alpha release; functionality may change.

This is a Laravel example project to show you how to use the [Flow PHP SDK](https://github.com/mayvenstudios/flow-php-sdk)


## Installation

### Composer

```
composer update
```

### Environment variables

After this, you should add the following variables in your .env file.
This example shows the default Flow CLI path for macOS if you're using Homebrew, but on a Linux server it will likely be `~/.local/bin`

```
FLOW_PATH=/opt/homebrew/bin/
FLOW_NETWORK=testnet
```

### Flow CLI

In order to interact with the blockchain you will need to install the [Flow CLI](https://docs.onflow.org/flow-cli/install/)

On macOS
```
brew install flow-cli
```

On Linux
```
sh -ci "$(curl -fsSL https://storage.googleapis.com/flow-cli/install.sh)"
```


## Example Usage


### Artisan Tinker

If you run the following command in Tinker

```
php artisan tinker
>>> use Flow;
>>> Flow::getLatestBlock();
```

You will see an output similar to this one

```
{"blockId":"e72ad32296fc39ab3f6ebebdf94fe952b64b3ce3a73d41e7e3f69b3024edd7e5","collection":[],"height":35167286,"parentId":"6ea1874dbceffa3eab986b3137347457d5d54f1e41b6a0ec74617756cc73c378","totalCollections":0,"totalSeals":0}
```

## Reference

Please check the [Flow-PHP-SDK](https://github.com/mayvenstudios/flow-php-sdk) page for all the available commands.


## License

[Apache License 2.0](http://www.apache.org/licenses/)
