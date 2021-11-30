<!--
IMPORTANT:

This repository contains configuration for what users see when they click on the `Actions` tab and the setup page for Code Scanning.

It is not:
* A playground to try out scripts
* A place for you to create a workflow for your repository
-->

---

## Tasks

**For _all_ workflows, the workflow:**

- [ ] Should be contained in a `.yml` file with the language or platform as its filename, in lower, [_kebab-cased_](https://en.wikipedia.org/wiki/Kebab_case) format (for example, [`docker-image.yml`](https://github.com/actions/starter-workflows/blob/main/ci/docker-image.yml)).  Special characters should be removed or replaced with words as appropriate (for example, "dotnet" instead of ".NET").
- [ ] Should use sentence case for the names of workflows and steps (for example, "Run tests").
- [ ] Should be named _only_ by the name of the language or platform (for example, "Go", not "Go CI" or "Go Build").
- [ ] Should include comments in the workflow for any parts that are not obvious or could use clarification.

**Some general notes:**

- [ ] This workflow must _only_ use actions that are produced by GitHub, [in the `actions` organization](https://github.com/actions), **or**
- [ ] This workflow must _only_ use actions that are produced by the language or ecosystem that the workflow supports.  These actions must be [published to the GitHub Marketplace](https://github.com/marketplace?type=actions).  We require that these actions be referenced using the full 40 character hash of the action's commit instead of a tag.  Additionally, workflows must include the following comment at the top of the workflow file:
    ```
    # This workflow uses actions that are not certified by GitHub.
    # They are provided by a third-party and are governed by
    # separate terms of service, privacy policy, and support
    # documentation.
    ```
- [ ] Automation and CI workflows should not send data to any 3rd party service except for the purposes of installing dependencies.
- [ ] Automation and CI workflows cannot be dependent on a paid service or product.
