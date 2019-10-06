# flux-experiment-helm-repo

# add a new chart

```bash
$ helm package <path_to_chart>/ # build the tgz file and copy it here
$ helm repo index . # create or update the index.yaml for repo
$ git add .
$ git commit -m 'add new chart'
```

# use the repo

```bash
$ helm repo add sample 'https://raw.githubusercontent.com/oschira/flux-experiment-helm-repo/master/'
$ helm repo update
$ helm search <chart>
```
