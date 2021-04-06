---
marp: true
theme: gaia
_class: lead
paginate: true
backgroundColor: #fff
backgroundImage: url('./assets/hero-background.jpg')
---

![bg left:40% 80%](https://raw.githubusercontent.com/NixOS/nixos-artwork/master/logo/nix-snowflake.svg)

# The Joy of Nix

---

# Nix:

* First debuted in 2006
* Powerful, mature package manager
* Extensive repository of up-to-date software packages
* Thriving community of active contributors
* Ecosystem of tightly integrated CI/CD solutions ...
* NixOS: a full Linux distribution that levarages all of the above

---

# Zealous marketing speak? 🤔

* Can I depend on Nix?
* Does Nix support my use case?
* Is Nix just an intellectual curiosity?
* If not, what sets it apart?

---

# Industry Adoption

* Atlassian
* Mozilla
* Target
* LumiGuide
* Tweag I/O
* Serokell
* Obsidian Systems

---

# Top Repositories

By **total** number of packages

|#|Repository   |Packages|
|-|-------------|-------:|
|1|AUR          |  59,965|
|2|nix          |  56,153|
|3|Debian+derivs|  34,671|

---

# Top Repositories

By number of **non-unique** packages

|#|Repository   |Packages|
|-|-------------|-------:|
|1|nix          |  48,885|
|2|AUR          |  27,932|
|3|Debian+derivs|  25,911|

---

# Top Repositories

By number of **maintainers**

|#|Repository   |Packages|
|-|-------------|-------:|
|1|AUR          |  10,520|
|2|Debian+derivs|   4,108|
|3|nix          |   1,677|

---

# Stats

* **Nix:** 33 packages per maintainer
* **Debian:** 8 packages per maintainer

---

<!-- _class: invert -->
<!-- backgroundImage: url('./assets/hero-background-inverted.jpg') -->

# Nix enables its users to be over 4x as effective!

---

<!-- backgroundImage: url('./assets/hero-background.jpg') -->

## Maybe nix packages are out of date? 🤔

---

# Top Repositories

By number of projects with up to date packages

|#|Repository   |Packages|
|-|-------------|-------:|
|1|nix          |  25,314|
|2|Debian+derivs|  17,047|
|3|FreeBSD Ports|  16,623|

---

<!-- _class: invert -->
<!-- backgroundImage: url('./assets/hero-background-inverted.jpg') -->

# Some Conclusions

* Nix has a massive package set
* Nix enables its 1,000+ contributors to punch above their weight
* Nix packages are more up to date
* Security issues are dealt with swiftly

---

<!-- backgroundImage: url('./assets/hero-background.jpg') -->

# What sets Nix apart? (1/3)

* Software is built in a hermetic, 100% reproducible environment
* Nix vs Docker:
    * Docker just guarantees that you can pass around the built images
    A Dockerfile might build successfully today and then fail tomorrow e.g. due to internet resources disappearing or the base image changing in an incompatible way
    * Nix guarantees that *both* the build process and resulting artifacts are reproducible.

---

# What sets Nix apart? (2/3)

* You can create deterministic development environments (without the awkwardness of developing inside of a container or VM)
    * You can lock specific versions of dev tools, C/C++ dependencies, etc
    * This applies per project; there is absolutely zero conflict with having one version used by one project and completely different version used in another project
* Superior visibility into the dependencies of your software (and your system as a whole)

---

# What sets Nix apart? (3/3)

* With NixOS, *the entire system state is reproducible*
    * Systemd services
    * Installed software
    * Network config
* A given NixOS config (with no changes) can be used for:
    * Network boot (iPXE)
    * Creating bootable ISOs
    * Installing on bare metal
    * Deployment to cloud providers

---

<!-- _class: invert -->
<!-- backgroundImage: url('./assets/hero-background-inverted.jpg') -->

# Demo Time

"We'll do it live!"