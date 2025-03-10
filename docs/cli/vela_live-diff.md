---
title: vela live-diff
---

Compare application and revisions

### Synopsis

Compare application and revisions

```
vela live-diff
```

### Examples

```
# compare the current application and the running revision
> vela live-diff my-app
# compare the current application and the specified revision
> vela live-diff my-app --revision my-app-v1
# compare two application revisions
> vela live-diff --revision my-app-v1,my-app-v2
# compare the application file and the specified revision
> vela live-diff -f my-app.yaml -r my-app-v1 --context 10
```

### Options

```
  -c, --context int         output number lines of context around changes, by default show all unchanged lines (default -1)
  -d, --definition string   specify a file or directory containing capability definitions, they will only be used in dry-run rather than applied to K8s cluster
  -e, --env string          specify environment name for application
  -f, --file string         application file name
  -h, --help                help for live-diff
  -n, --namespace string    specify the Kubernetes namespace to use
  -r, --revision string     specify one or two application revision name(s), by default, it will compare with the latest revision
```

### Options inherited from parent commands

```
  -y, --yes   Assume yes for all user prompts
```

### SEE ALSO



#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by spf13/cobra on 19-Apr-2022, refer to [script in KubeVela](https://github.com/oam-dev/kubevela/tree/master/hack/docgen).
