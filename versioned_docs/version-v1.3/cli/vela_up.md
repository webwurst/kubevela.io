---
title: vela up
---

Deploy one application

### Synopsis

Deploy one application

 Deploy one application based on local files or re-deploy an existing application. With the -n/--namespace flag, you can choose the location of the target application.

 To apply application from file, use the -f/--file flag to specify the application file location.

 To give a particular version to this deploy, use the -v/--publish-version flag. When you are deploying an existing application, the version name must be different from the current name. You can also use a history revision for the deploy and override the current application by using the -r/--revision flag.

```
vela up
```

### Examples

```
  # Deploy an application from file
  vela up -f ./app.yaml
  
  # Deploy an application with a version name
  vela up example-app -n example-ns --publish-version beta
  
  # Deploy an application using existing revision
  vela up example-app -n example-ns --publish-version beta --revision example-app-v2
```

### Options

```
  -e, --env string               The environment name for the CLI request
  -f, --file string              The file path for appfile or application. It could be a remote url.
  -h, --help                     help for up
  -n, --namespace string         If present, the namespace scope for this CLI request
  -v, --publish-version string   The publish version for deploying application.
  -r, --revision string          The revision to use for deploying the application, if empty, the current application configuration will be used.
```

### Options inherited from parent commands

```
  -y, --yes   Assume yes for all user prompts
```

### SEE ALSO



#### Go Back to [CLI Commands](vela) Homepage.


###### Auto generated by spf13/cobra on 19-Apr-2022, refer to [script in KubeVela](https://github.com/oam-dev/kubevela/tree/master/hack/docgen).
