# Mac-nodejs-npm-setup
Setting up Nodejs and NPM on macOS to avoid permissions error


# Download NodeJs
https://nodejs.org/en/

# Create a global npm dir
mkdir ~/.npm-global

# Config npm to user dir
npm config set prefix '~/.npm-global'

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
