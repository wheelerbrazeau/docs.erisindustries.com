---

layout:     documentation
title:      "Documentation | eris:cli | eris update"

---

# eris update

Update the eris tool.

## Synopsis

Fetch the latest version (master branch by default)
and re-install eris. Once eris is reinstalled, then the
eris init function will be called automatically for you
in order to update your definition files and images.

If you have made modifications to the default definition files
then you will want to make backups of those **before** upgrading
your eris installation.

```bash
eris update
```

## Options

```
  -b, --branch string   specify a branch to update from (default "master")
      --pull-images     by default, pulls and/or update latest primary images. use flag to skip pulling/updating of images. (default true)
      --source string   source from which to download definition files for the eris platform. if toadserver fails, use: rawgit (default "rawgit")
      --yes             over-ride command-line prompts
```

## Options inherited from parent commands

```
  -d, --debug            debug level output
  -m, --machine string   machine name for docker-machine that is running VM (default "eris")
  -v, --verbose          verbose output
```

## See Also

* [eris](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/eris/)	 - The Blockchain Application Platform

## Specifications

* [Actions Specification](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/actions_specification/)
* [Chains Specification](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/chains_specification/)
* [Contracts Specification](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/contracts_specification/)
* [Motivation](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/motivation/)
* [Services Specification](https://docs.erisindustries.com/documentation/eris-cli/0.11.4/services_specification/)

