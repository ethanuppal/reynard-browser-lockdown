# reynard-browser-lockdown

This disables the lockdown mode check for JIT in Reynard Browser.
It is useful for those who use lockdown mode not to avoid cyberattacks but to safely stay on older versions of iOS, where the main issue is WebKit becoming outdated.

The submodule [`reynard-browser`](./reynard-browser/) is just a convenience.
The [build workflow](./.github/workflows/build.yaml) automatically checks out the latest nightly Reynard in the submodule on a cron job and builds it.

IMPORTANT TODO:
- [ ] Pin all the workflow actions to commit hash
- [ ] Run `zizmor` to make sure everything is ok

TODO:
- [x] It should see if it already published the latest version and skip
- [x] Add an additional patches folder whose contents are copied into the Reynard patches before building
- [ ] Add an extra hash so we can add new patches and be able to release a new version based on the same version of Reynard
- [ ] Add sourcegen to workflow

BIG TODO:
- It would be nice if we could have a global or per site toggle like Safari does
