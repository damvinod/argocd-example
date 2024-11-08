# ArgoCD Hands-on Practice
1) Follow steps 1 to 4 from [the docs](https://argo-cd.readthedocs.io/en/latest/getting_started/) to install and login to ArogoCD using the port forward.
2) Create a new Repository by giving the below details
   - Choose your connection method: via HTTPS
   - Type - git
   - Repository URL: https://github.com/damvinod/argocd-example.git
3) Create the below projects and give the wildcard permissions(*) to SOURCE REPOSITORIES and for DESTINATIONS choose https://kubernetes.default.svc.
  - demo-dev
  - demo-stg


## Create Application

### Dev Env
- Click on New App and choose Edit As YAML and copy [this](https://github.com/damvinod/argocd-example/blob/main/argocd-application/dev/application-dev.yaml) contents to create guestbook application in demo-dev project

### STG ENV
- Click on New App and choose Edit As YAML and copy [this](https://github.com/damvinod/argocd-example/blob/main/argocd-application/stg/application-stg.yaml) contents to create guestbook application in demo-stg project

## Create ApplicationSet

-  Click on New App and choose Edit As YAML and copy [this](https://github.com/damvinod/argocd-example/blob/main/argocd-application/application-for-app-set.yaml) contents to create visitorbook application in demo-dev, demo-stg project