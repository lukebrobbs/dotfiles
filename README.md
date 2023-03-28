# Dotfiles

These are my config files used on my development machines. 

I am utilizing [chezmoi](https://www.chezmoi.io). To get started, you will need to download the `dotlaptop.local` file:

```bash
cd ~
curl --remote-name https://raw.githubusercontent.com/lukebrobbs/dotfiles/main/dot_laptop.local
mv dot_laptop.local .laptop.local
./.laptop.local
```

## Other tools to install

### Oh My Zsh

```bash
sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
```

## On the new machine

Once all your machines are set up, keeping the dotfiles in sync between them is very easy. If you make any changes to the dotfiles on one machine, you push them to GitHub, and then all you have to do on the other machines is:

```bash
chezmoi update
```