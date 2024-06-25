# asdf

 ---
 
 ### Installation Instructions
 
 #### Install prerequisites
 ```sh
 sudo apt install curl git
 ```
 
 #### Clone the asdf repository
 ```sh
 git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
 ```
 
 #### Update your shell configuration
 Add the following lines to your `~/.bashrc`:
 ```sh
 . "$HOME/.asdf/asdf.sh"
 . "$HOME/.asdf/completions/asdf.bash"
 ```
 Then, reload your `~/.bashrc`:
 ```sh
 source ~/.bashrc
 ```
 
 ### Install Node.js
 ```sh
 sudo apt-get install dirmngr gpg curl gawk
 asdf plugin add nodejs https://github.com/asdf-vm/asdf-nodejs.git
 asdf install nodejs latest
 ```
 
 ### Install Ruby
 ```sh
 asdf plugin add ruby https://github.com/asdf-vm/asdf-ruby.git
 ```
 
 #### Verify the installation
 Correct output from `type -a ruby` (asdf shim is first in the list):
 ```sh
 ruby is /Users/someone/.asdf/shims/ruby
 ruby is /usr/bin/ruby
 ```
 
 Incorrect output from `type -a ruby`:
 ```sh
 ruby is /usr/bin/ruby
 ```
 
 ---
