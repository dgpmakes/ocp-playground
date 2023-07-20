# Index
1. Installing Openshift Pipelines
2. Tasks


## 1. Installing Openshift Pipelines
** work in progress**
## 2. Tasks
We will use an ArgoCD instance that deploys an app that deploys other apps.

#### 1. Add user to system

This task creates a user, managing secrets automatically. It needs two parameters: the name of the use and its password.
To use this task, the SA for pipelines needs permission to access the secrets of openshift-config.
```bash
oc policy add-role-to-user cluster-admin system:serviceaccount:pipelines-test:pipeline -n openshift-config
```

#### 2. Copy secret to another namespace
** work in progress**
