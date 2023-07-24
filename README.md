# Test Charts Repository

## Objective

Smaller fork of `rancher/charts` for making testing the repository chart functionality within `rancher/rancher` easier and faster.

Most of the charts and files were removed because they are not necessary for testing the functionalities. 

### Architecture

- 2 Branches for testing `Ensure Head and Update` methods from `rancher/pkg/catalogv2/git`. 
    - Branch: `main`
        - Charts
        1. `fleet` until version: `102.1.0+up0.7.0`
        2. `fleet-agent` until version: `102.1.0+up0.7.0`
        3. `fleet-crd` until version: `102.1.0+up0.7.0`
        4. `rancher-webhook` until version: `2.0.5+up0.3.5`
        5. `rancher-cis-benchmark` until version: `4.0.0`
        6. `rancher-cis-benchmark-crd` until version: `4.0.0`
        7. `rancher-aks-operator` until version: `102.0.0+up1.1.0`
        8. `rancher-aks-operator-crd` until version: `102.0.0+up1.1.0`
    - Branch: `test-1`
        - Charts
        1. `fleet` until version: `102.0.0+up0.6.0`
        2. `fleet-agent` until version: `102.0.0+up0.6.0`
        3. `fleet-crd` until version: `102.0.0+up0.6.0`
        4. `rancher-webhook` until version: `2.0.3+up0.3.3`
        5. `rancher-cis-benchmark` until version: `3.0.0`
        6. `rancher-cis-benchmark-crd` until version: `3.0.0`
        7. `rancher-aks-operator` until version: `101.0.0+up1.0.7`
        8. `rancher-aks-operator-crd` until version: `101.0.0+up1.0.7`