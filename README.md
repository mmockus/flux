# flux


## Deployed CLI with Ansible

- [mmockus/ansible - dev-host.yml](https://github.com/mmockus/ansible/blob/main/playbooks/dev-host.yml)

## Flux bootstrap

run from where you can run flux/kubectl

```
flux bootstrap github \
  --components-extra=image-reflector-controller,image-automation-controller \
  --owner=mmockus \
  --repository=flux \
  --branch=main \
  --path=clusters/home \
  --personal \
  --token-auth 
```  

## References

- [Techno Tim - The FASTEST way to deploy apps to Kubernetes - GitOps with FLUX](https://docs.technotim.live/posts/flux-devops-gitops/)