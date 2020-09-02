# First of all.
 You Must Close All Chrome Windows Before Applying The Steps Below

<br>

# Linux 🐧🐧

1. run this command 

        sudo gedit /usr/share/applications/google-chrome.desktop

2. add the line below to the end of 
the lines starting with the word `Exec`

        --disable-web-security --disable-gpu  --user-data-dir --allow-file-access-from-files

so the final result line is like that:

    Exec=/usr/bin/google-chrome-stable %U --disable-web-security --disable-gpu  --user-data-dir --allow-file-access-from-files

<br>

# Windows 

1- make a shortcut from the original `chrome.exe`
- You can find it by
    1. open a new tab in google chrome and enter this `chrome://version/`
    2. the full path is at `Executable Path` 

2- Right-click on the shortcut Add This To The `Target (section)` in the `Shortcut (tab)`

        --disable-web-security --disable-gpu  --user-data-dir --allow-file-access-from-files

so the final result line is like that:


    "C:\Program Files (x86)\Google\Chrome\Application\chrome.exe" --disable-web-security --disable-gpu  --user-data-dir --allow-file-access-from-files

<br>

# DONE 😎