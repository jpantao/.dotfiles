# Dotfiles
 This is a bare git repository that I use to manage my dotfiles.

All the information here is in more detail in: [The best way to store your dotfiles](https://www.atlassian.com/git/tutorials/dotfiles)

1. **First you will need the alias:**
   `alias dotfiles="/usr/bin/git --git-dir=$HOME/.dotfiles/ --work-tree=$HOME"`

1. **Clone the repo into your home directory
   `git clone --bare  https://github.com/jpantao/.dotfiles.git $HOME/.dotfiles`

1. **Then checkout the contents from the repository to your home directory:**
   `dotfiles checkout`

   This is likely fail because you might already have configuration files that would be overwritten. Just backup the files or simply remove them and repeat the checkout.

1. **Set the showUntrackedFiles flag to no:**
   `dotfiles config --local status.showUntrackedFiles no`

1. **Pulling updates:**
   `dotfiles pull`


## Dependencies:
   - [Fira Code](https://github.com/tonsky/FiraCode).
   - [Fish shell](https://fishshell.com/).
   - [Oh My Fish](https://github.com/oh-my-fish/oh-my-fish).