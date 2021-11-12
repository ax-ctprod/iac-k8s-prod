# iac-k8s-prod
On-disk configs now in repository for team management.

## Prep

* kubectl
* k8s token portal access

## Usage

    # run after cluster terraforms
    #
    # SSO+download your kubeconfig from the portal
    #   if not already done.

    # for prod
    kubectl apply -f be.yaml -s ct-k8s-prod.asint.automox.com:6443

    # for dev (must be on VPN)
    kubectl apply -f be.yaml -s ct-k8s-dev.asint.automox.com:6443

