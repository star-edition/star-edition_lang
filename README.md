
# Documentation

## Initial setup
Create a directory and open it in Git Bash:
```
    git init
    git pull https://github.com/star-edition/star-edition_lang.git
    git remote add origin https://github.com/star-edition/star-edition_lang.git
```
You should now have the localization files in the directory!

## Main Translation
Add/change or remove translation entries in the chosen language file (e.g. `ru_RU.lang`).

You may use comparing tools such as https://text-compare.com/ to compare the main file `en_US.lang` with your language file and change accordingly.

However, with the new git system in use for the localization files, it is recommended to edit language files based on commits to the main file. There are three types of changes to be seen in the commit messages for ease:
```
    ADD = an entry was added
    CHN = an entry was changed
    REM = an entry was removed
```

## Pushing changes
After you have made your changes, open the directory in Git Bash and do the following:
```
    git commit -a -m "[YOUR MESSAGE HERE]"
    git push
```
*(Use `git push --set-upstream origin master` if you're pushing for the first time).*\
You should now see the changes on the Github site.

## Retrieving changes
To retrieve the most recent version of the repository, open the directory in Git Bash and run the following:
```
    git pull
```


