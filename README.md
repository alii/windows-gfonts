# windows-gfonts
Batch install instructions to install every google font ever.

1. Download the entire Google Font repo by going [here](https://github.com/google/fonts) and either cloning with `git clone` or downloading as a Zip file.
2. If you downloaded as a Zip, extract all the subdirectories of the archive from folder `otf` to another directory locally on your machine. The folder `otf` just contains all the fonts.
3. The problem we have now is, the fonts are all in their own directory. This is a huge pain to install manually. Luckily, we have a solution. Open the directory containing all the font directories and then **shift+right click** in windows explorer. Hit open command prompt here.
4. Type in `xcopy *.ttf DESTINATION /s` where `DESTINATION` is another directory on your machine. Do not use the directory you are already in, since it will mess up the next step.
5. Fantastic! All your ttf files are now on their own inside their own folder, but we still can't drag and drop install them. We must now close down Command Prompt and bring up your explorer window once again. In the search bar, type `NOT kind:folder`. You should now see a list of ttf files! Open another explorer window to `Control Panel\All Control Panel Items\Fonts` and then drag all of the fonts into that window.
6. Profit!
