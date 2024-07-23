# Charts Small Fork

## Objective

Helm Repository to be used by rancher for testing Mapps teams functionalities.

Cloning the original repository (`rancher/charts`) takes time due to its size,
also, the repository is always being updated which makes it harder for hard-coding values to be tested.

This repository is like a freeze in time with very few charts for the cloning at our Drone testing pipeline to be as fast as it can while allowing hard-coded values in the tests.

This repository is not used to test the **specific Chart functionalities**.
e.g: We test changing branches of the repository which holds different chart versions and if the available charts gets the newer versions.

This repository should only be similar to the `rancher/charts` structure with very few charts so we don't add more time to the Drone build pipeline.

---

### Directives

- **DO NOT EDIT** the branches `main` and `test-1`.
- They are being used on automated integrated and unit tests.
- You are free to add any other branches.

---

#### How-to-use

- 2 Branches for testing `Ensure Head and Update` methods from `rancher/pkg/catalogv2/git`.
    - Branch: `main`
        - Charts
        1. `fleet` until version: `102.1.0+up0.7.0-rc.2`
        2. `fleet-agent` until version: `102.1.0+up0.7.0-rc.2`
        3. `fleet-crd` until version: `102.1.0+up0.7.0-rc.2`
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
    - Branch: `aks-integration-test-working-charts`
        - Charts used in tests:
        1. `rancher-aks-operator` version: `104.0.2+up1.9.0` (working)
        2. `rancher-aks-operator-crd` version: `104.0.2+up1.9.0` (working)