# Victor's Dotfiles

This repo is here to simplify my process of getting a new machine "dev ready". It also serves as a handy outline of tools / applications that I use in my day to day work.

## Instructions

**If upgrading / migrating from a different machine, dont forget to:**

- Go over all Sites / Apps that I'm workign on, make sure the latest changes have been pushed to Github / Bitbucket.
- Backup databases of sites I'm working on.
- Backup `~/.ssh` directory
- for all Shopify sites built with Slate, backup `.env` and `.env.production` files

**On a new environment:**

1. Update macOS to the latest version via App Store
2. Install macOS Command Line Tools by running `xcode-select --install`
3. Clone this repo to `~/.dotfiles`
4. Install [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh)
5. Go to dotfiles dir. `cd ~/.dotfiles` and run `sh install.sh` to initiate the setup
6. Restart the computer after everything is done

## Caveats

1. Homebrew will claim **VirtualBox** installation has failed, in reality, it will install but will need user to manually authorize it from `System Prefs » Security & Privacy`.
   See: [Github Issue](https://github.com/Homebrew/homebrew-cask/issues/63083), [Medium Post](https://medium.com/@Aenon/mac-virtualbox-kernel-driver-error-df39e7e10cd8)
   **Note:** Security settigns will need to be updated within 30min of install / first launch, otherwise opt. disappears. If you done goofed, you will need to uninstall & re-install VirtualBox. Follow instructions here for complete [VirtualBox Uninstall](https://nektony.com/how-to/uninstall-virtualbox-on-mac).

2. **MySQL & WordPress** when testing these scripts, WordPress would refuse to connect to MySQL db, even though connecting to it using the same credentials via command line was fine. [This comment](https://discourse.brew.sh/t/homebrew-php-7-4-upgrade-fails-on-macos-10-15-1-catalina/6372/14) of the thread solved the issue.

## Acknowledgements

My dotfiles are largely based upon [Dries Vints](https://github.com/driesvints) dotfiles [repo](https://github.com/driesvints/dotfiles).

Much thanks to [Dries Vints](https://github.com/driesvints), [Mathias Bynens](https://github.com/mathiasbynens/dotfiles) whose dotfile repos served as a source of knowledge & inspiration for my own setup.
