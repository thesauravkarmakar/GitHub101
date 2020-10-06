# Windows
On Windows, the GitHub CLI is available via [Scoop](https://scoop.sh/), [Chocolatey](https://chocolatey.org/), and as downloadable MSI.
#### scoop

Install:

```powershell
scoop bucket add github-gh https://github.com/cli/scoop-gh.git
scoop install gh
```

Upgrade:

```powershell
scoop update gh
```

#### Chocolatey

|Install:|Upgrade:|
|---|---|
|`choco install gh`|`choco upgrade gh`|

#### MSI

MSI installers are available for download on the ![releases page](https://github.com/cli/cli/releases/latest).

You install these as you would any other program

# MacOS


On MacOS, the CLI is available via Homebrew and MacPorts.
gh

|Install:|Upgrade:|
|---|---|
|`brew install gh`|`brew upgrade gh`|

#### MacPorts

|Install:|Upgrade:|
|---|---|
|`sudo port install gh`|`sudo port selfupdate && sudo port upgrade gh`|

# Linux

The Linux installation is platform-dependant, whereas you need to know your distribution and follow the instructions accordingly 

### Debian, Ubuntu Linux (apt)

Install:

```bash
sudo apt-key adv --keyserver keyserver.ubuntu.com --recv-key C99B11DEB97541F0
sudo apt-add-repository https://cli.github.com/packages
sudo apt update
sudo apt install gh
```

**Note**: If you are behind a firewall, the connection to `keyserver.ubuntu.com` might fail. In that case, try running `sudo apt-key adv --keyserver hkp://keyserver.ubuntu.com:80 --recv-key C99B11DEB97541F0`.

**Note**: If you get _"gpg: failed to start the dirmngr '/usr/bin/dirmngr': No such file or directory"_ error, try installing the `dirmngr` package. Run `sudo apt-get install dirmngr` and repeat the steps above.  

**Note**: most systems will have `apt-add-repository` already. If you get a _command not found_
error, try running `sudo apt install software-properties-common` and trying these steps again.


Upgrade:

```bash
sudo apt update
sudo apt install gh
```

### Fedora, CentOS, Red Hat Enterprise Linux (dnf)

Install:

```bash
sudo dnf config-manager --add-repo https://cli.github.com/packages/rpm/gh-cli.repo
sudo dnf install gh
```

Upgrade:

```bash
sudo dnf update gh
```

### openSUSE/SUSE Linux (zypper)

Install:

```bash
sudo zypper addrepo https://cli.github.com/packages/rpm/gh-cli.repo
sudo zypper ref
sudo zypper install gh
```

Upgrade:

```bash
sudo zypper ref
sudo zypper update gh
```

### openSUSE/SUSE Linux (zypper)
 
Install and upgrade:

1. Download the `.rpm` file from the![releases page](https://github.com/cli/cli/releases/latest);
2. Install the downloaded file: `sudo zypper in gh_*_linux_amd64.rpm`

## Community-supported methods

Our team does not directly maintain the following packages or repositories. They are unofficial and we are unable to provide support or guarantees for them.

### Arch Linux

Arch Linux users can install from the ![community repo](https://aur.archlinux.org/packages/github-cli-git):

```bash
sudo pacman -S github-cli
```

### Android

Android users can install via Termux:

```bash
pkg install gh
```

### Kiss Linux

Kiss Linux users can install from the [community repos](https://github.com/kisslinux/community):

```bash
kiss b github-cli && kiss i github-cli
```

### Nix/NixOS

Nix/NixOS users can install from [nixpkgs](https://search.nixos.org/packages?show=gitAndTools.gh&query=gh&from=0&size=30&sort=relevance&channel=20.03#disabled):

```bash
nix-env -iA nixos.gitAndTools.gh
```
