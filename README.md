# Home Manager

My `home-manager` config. Currently only using this for WSL.

1. Install WSL with Ubuntu (comes with systemd enabled)
2. Install Nix and enable flakes
3. Clone this repo to `~/.config/home-manager` and run:

   ```bash
   nix shell nixpkgs#home-manager
   home-manager switch
   ```

FIXME: To get zsh working in WSL I had to run the following.

```bash
sudo chsh -s /home/fng/.nix-profile/bin/zsh
chsh -s /home/fng/.nix-profile/bin/zsh
```

## Todos

- fix clipboard (search for `wsl` in `:help clipboard`)
- change themes to ayu (would be cool if nvim could inherit wezterm theme)
- unify neovim and zellij pane movement
  - https://www.reddit.com/r/zellij/comments/18xz5ng/use_alt_for_keybinds_in_zellij_avoid_conflicts/
  - https://github.com/swaits/zellij-nav.nvim
- scrolling from keyboard in terminal?
