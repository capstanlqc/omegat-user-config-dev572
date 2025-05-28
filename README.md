# OmegaT configuration

OmegaT's default factory settings (namely, interface and behaviour preferences) are not suitable for all kinds of tasks. They can be tweaked and customized, but doing so by hand one by one may be tedious and error-prone, especially for large teams where preferences are expected to be homogeneous across the whole team.

This is a collection of tweaked configuration files where the most convenient value for every option has been chosen, as well as some extensions (scripts and plugins). This is the configuration that OmegaT users need to work in cApStAn projects or in projects where cApStAn provides translation technology support. The purpose is to spare those users the burden of tweaking their configuration manually.

## Installing and setting up OmegaT

This configuration is installed automatically in cApStAn's custom build of OmegaT. If you're an intended user of that version of OmegaT, please refere to [this guide](https://capstanlqc.github.io/omegat-guides/translation/install-and-setup/). You don't need to use this repository at all -- it is kept public for transparency purposes but is only meant for internal use by cApStAn.


## Disclaimer

This configuration is meant to be used exlusively with cApStAn's custom build of OmegaT, which deliberately uses a custom configuration folder to that effect, by cApStAn subcontractors or by linguists participating in projects where cApStAn provides support in terms of translation technology. 

> [!CAUTION]
> Do not use this configuration (and scripts in particular) with any OmegaT version other than 
cApStAn's custom build of OmegaT. Do not add files from this repository to your OmegaT configuration, that is not the intended way of using this configuration. You may experience configuration incompatibility problems if you ignore this warning and do the above.


## For maintainers (INTERNAL): how to update this repository

Between releases: 

1. Add/update/remove whatever config/script/plugin files as needed
2. Update the `changes.md` file with a description of the updates, under the next release header

When a new release is ready: 

3. Make sure the next update header has:

	- a number that is +1 higher than the previous update
	- a correct `csp` indication of what exactly is being updated: 
		- the first letter is mandatorily `c` (config)
		- the second letter is `s` if there are updates in scripts, otherwise `0`
		- the third letter is `p` if there are updates in plugins, otherwise `0`
	- the date of the expected release

Example: `## Update 98_cs0 (2024-02-28)`


<!-- 
```
bash -c "$(curl -fsSL https://raw.githubusercontent.com/capstanlqc/omegat-setup/master/custo/omtlinux_custom_installer.sh)"
```
-->

<!-- @TODO: write instructions for chocolatey in PowerShell -->
