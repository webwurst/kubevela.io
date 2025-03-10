---
title: vela trait
---

List/get traits.

### Synopsis

List trait types installed and discover more in registry.

```
vela trait [flags]
```

### Examples

```
vela trait
```

### Options

```
      --discover                       discover traits in registries
  -h, --help                           help for trait
      --label --label type=terraform   a label to filter components, the format is --label type=terraform
      --registry string                specify the registry name (default "default")
      --token string                   specify token when using --url to specify registry url
      --url string                     specify the registry URL
```

### Options inherited from parent commands

```
  -y, --yes   Assume yes for all user prompts
```

### SEE ALSO


* [vela trait get](vela_trait_get)	 - get trait from registry

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by spf13/cobra on 19-Apr-2022, refer to [script in KubeVela](https://github.com/oam-dev/kubevela/tree/master/hack/docgen).
