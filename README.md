# lastdl

Put the lastdl script somewhere on your path:


    $ cat ~/bin/lastdl
    #!/usr/bin/env bash
    echo -n "$HOME/Downloads/"
    ls -t "$HOME/Downloads" | head -n 1


You can use it like this, its really easy to manipulate the latest download.

    $ lastdl
    /home/oscar/Downloads/photos-20230613.WxJw9t3d.zip.part

Example: copy last downloaded file to current directory.

    $ cp $(lastdl) .
