# How to install NodeJS and NPM on MacOS
Follow the instructions below to avoid permissions errors when installing
NPM packages on your mac.
---
## Download NodeJs
Download and install NodeJS if you haven't already.
https://nodejs.org/en/
---
## Create a new npm global directory
Create a new npm global directory for your npm packages
`mkdir ~/.npm-global`

# Config npm to user dir
npm config set prefix '~/.npm-global'
double check the path config
npm list -g --depth=0

# Create a .zshrc file
Open Terminal
Type touch ~/.zshrc to create the respective file. (touch command will create the .zshrc in your current directory but it will be hidden)
Hit Return

To view/open ~/.zshrc you can do either of two things:

Open Finder > Press Cmd+Shift+.
Or:

Open Terminal > and type: open ~/.zshrc

# Export the path to npm global dir
Open the .zshrc and add this line:
export PATH=~/.npm-global/bin:$PATH

Open Terminal and source the .zshrc file
source ~/.zshrc

double check
echo $PATH
