# FluxCD HelpFul Documents

## Flux Bootstrap Cheatsheet

https://fluxcd.io/flux/cheatsheets/bootstrap/

## Github Git Bootstrap

```FluxGithubSync
https://fluxcd.io/flux/installation/#github-and-github-enterprise

Create a PAT and export it.

flux bootstrap github \
  --owner=elkosmonaut \
  --repository=repoName \
  --path=pathInTheRepo \
  --personal
```

## Forge Bootstrap

```notes
Instead of bootstrapping anything, install the flux componets into the cluster and then create the things you need.  As long as the source controller, kustomization controller, helm controller, etc make it into the cluster you create the repo/secrets/permissions/deploykeys and those controllers will use the resources you create.
```

1) GitRepository
2) Kustomization
