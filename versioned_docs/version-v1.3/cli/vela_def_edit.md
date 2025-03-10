---
title: vela def edit
---

Edit X-Definition.

### Synopsis

Edit X-Definition in kubernetes. If type and namespace are not specified, the command will automatically search all possible results.
By default, this command will use the vi editor and can be altered by setting EDITOR environment variable.

```
vela def edit NAME [flags]
```

### Examples

```
# Command below will edit the ComponentDefinition (and other definitions if exists) of webservice in kubernetes
> vela def edit webservice
# Command below will edit the TraitDefinition of ingress in vela-system namespace
> vela def edit ingress --type trait --namespace vela-system
```

### Options

```
  -h, --help               help for edit
  -n, --namespace string   Specify which namespace to get. If empty, all namespaces will be searched.
  -t, --type string        Specify which definition type to get. If empty, all types will be searched. Valid types: trait, policy, workload, scope, workflow-step, component
```

### Options inherited from parent commands

```
  -y, --yes   Assume yes for all user prompts
```

### SEE ALSO

* [vela def](vela_def)	 - Manage Definitions

#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by spf13/cobra on 19-Apr-2022, refer to [script in KubeVela](https://github.com/oam-dev/kubevela/tree/master/hack/docgen).
