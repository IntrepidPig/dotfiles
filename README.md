## IntrepidPig's dotfiles

Each subfolder is a collection of dotfiles for a rice. To use a rice, clone the repo to `~/.config/dotfiles/`.

```
.config/
 |- dotfiles/
     |- FTL
     |- Flight
     |- ...
```

Then make a symlink to your preferred rice called default in `~/.config/dotfiles/`.

```
.config/
 |- dotfiles/
     |- FTL/
     |- Flight/
     |- ...
     |- default -> Flight
```

Now change all your config files to be symlinks to their respective file in `~/.config/dotfiles/default/`.
For example the file `~/.zshrc` would become a symlink to `~/.config/dotfiles/default/.zshrc`.
Do this for all of your config files you want to be part of the rice.

Now whenever you want to use a different setup you can just change the symlink at `~/.config/dotfiles/default` to point to a different rice, and all of the config files will now point to that rice.

