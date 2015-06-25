1: $`brew install rbenv ruby-build`

2: $`echo 'eval "$(rbenv init -)"' >> ~/.bash_profile` (replace `.bash_profile` with `.zshrc` if you're using zsh)

> Once you've completed the first two steps you can run the command $ `rbenv` which will give you a short list of rbenv commands. Rbenv is a ruby environment manager, which allows you to install multiple versions of Ruby.


## Why we need rbenv and our own version of Ruby.


> Every apple computer comes with a version of Ruby already installed (2.0.0). Your computer's OS uses Ruby to run various processes. So while itâ€™s not terrible to mess with the configuration of your systems Ruby i.e. changing permissions, sudo installing gems etc. Itâ€™s better just have our own version.   

> Also, consider this: if we have have Ruby 2.0.0 installed by default and we then install Ruby 2.2.0, how do we tell the computer which version of Ruby to use and in what instance? This is why we need an environment management tool   

## Steps 3 - 5


3: After you run $`rbenv` youâ€™ll see a list of commands like `rbenv versions`, `rbenv install`, `rebenv global` etc. We want to run $`rbenv install 2.2.0`
   
4: Run $`rbenv rehash`

5: Run $`rbenv global 2.2.0`

>Steps 3 through 5 install the Ruby version 2.2.0. Rehashing is a configuration process specific to rbenv. Rehash needs to be run after installing any new version of Ruby. The command `rbenv global 2.2.0` sets 2.2.0 to be the version thatâ€™s used globally on your computer. You may have also noticed `rbenv local`, which will set a ruby version specifc to a project, and `rbenv shell` which sets a specific ruby version to run in your terminal.

>You can read all about this and more about Rbenv, what it does and how to use it [here](https://github.com/sstephenson/rbenv):

