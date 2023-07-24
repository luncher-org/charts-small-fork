# Test Charts Repository

## Objective

Smaller fork of `rancher/charts` for making testing the repository chart functionality within `rancher/rancher` easier and faster.

Most of the charts and files were removed because they are not necessary for testing the functionalities. 

### Architecture

- 2 Branches for testing `Ensure Head and Update` methods from `rancher/pkg/catalogv2/git`. 
    - Branch: `main`
        - Charts
        1. `fleet` until version: `102.2.0+up0.8.0-rc.3`
        2. `fleet-agent` until version: `102.2.0+up0.8.0-rc.3`
        3. `fleet-crd` until version: `102.2.0+up0.8.0-rc.3`
        4. `rancher-webhook` until version: `2.0.6+up0.3.6-rc1`
        5. `rancher-cis-benchmark` until version: `4.0.0`
        6. `rancher-aks-operator` until version: `102.0.0+up1.1.0`
    - Branch: `test-1`
        - Charts
        1. `fleet` until version: `100.0.2+up0.3.8`
        2. `fleet-agent` until version: `100.0.2+up0.3.8`
        3. `fleet-crd` until version: `100.0.2+up0.3.8`
        4. `rancher-webhook` until version: `1.0.0+up0.2.0`
        5. `rancher-cis-benchmark` until version: `4.0.0`
        6. `rancher-aks-operator` until version: `102.0.0+up1.1.0`