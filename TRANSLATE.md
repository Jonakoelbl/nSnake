# Updating the PO/POT Files

From time to time, you might add a few strings into the original source files. 
If you do, you do not need to restart everything from scratch, you may simply merge what you have with the new strings.

We first need to update the .pot file (as previously):
```sh
    sudo make src/locale/GameStateMainMenu.pot
```

Then, we merge it with the previous src/locale/es/GameStateMainMenu.po file :
```sh
    sudo make src/local/es/GameStateMainMenu.po
```

Finally, we write the translation of the new string in the .po file and build the .mo file as follow:
```sh
    sudo make src/local/es/GameStateMainMenu.mo
```

