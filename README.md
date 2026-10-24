# reynard-browser-lockdown

This disables the lockdown mode check for JIT in Reynard Browser.

> [!CAUTION]
> You use this lockdown mode protection disabled at your own risk.
> Remember that JITs in browsers are the entry points of many serious attacks.

<h3 align="center">
<a href="https://altdirect.app/?url=https://www.ethanuppal.com/reynard-browser-lockdown/source.json" target="_blank"><img src="https://altdirect.app/assets/png/AltSource_Blue.png" alt="Add AltSource" width="200"></a>
&nbsp;
<a href="https://github.com/ethanuppal/reynard-browser-lockdown/releases/latest/" target="_blank"><img src="https://altdirect.app/assets/png/Download_Blue.png" alt="Download .ipa" width="200"></a>
</h3>

The submodule [`reynard-browser`](./reynard-browser/) is just a convenience.
The [build workflow](./.github/workflows/build.yaml) automatically checks out the latest stable Reynard in the submodule on a cron job and builds it.

IMPORTANT TODO:
- [x] Pin all the workflow actions to commit hash (except rust-toolchain)
- [x] Run `zizmor` to make sure everything is ok

TODO:
- [x] It should see if it already published the latest version and skip
- [x] Add an additional patches folder whose contents are copied into the Reynard patches before building
- [ ] Add an extra hash so we can add new patches and be able to release a new version based on the same version of Reynard
- [x] Add sourcegen to workflow

BIG TODO:
- It would be nice if we could have a global or per site toggle like Safari does
