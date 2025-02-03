__Dependency command:__ sudo apt-get -y install curl net-tools jq netcat-openbsd unzip wget git vim fail2ban imagemagick-6.q16 build-essential sqlite3 openssh-client

Note: netcat needed to be updated to netcat-openbsd.

__Moving the golang file:__ You need to use scp to move the golang file from your PC to /usr/local/ on your Pi, which gave me permission denied issues.

Doing `sudo chmod 777 /usr/local` fixed this by giving "others" permission to modify this folder, but this is bad practice. Find better solution or include reversion of permissions `sudo chmod 755 /usr/local` after doing so in any script.

__go needs PATH:__ `export PATH=$PATH:/usr/local/go/bin`after untarring the golang file.

__go needs a different install?:__ <https://go.dev/doc/install> 

<https://golangdocs.com/install-go-linux> `source .profile` should be `source $HOME/.profile`

<https://splitunknown.medium.com/installing-go-golang-on-linux-macos-and-windows-a-step-by-step-guide-7efe0643123b>

__golang is annoying:__ Scratch all of the above, replace golang install with `sudo apt -y install golang`