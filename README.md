# Jon Yard

Github pages hosted site using [Jekyll](https://jekyllrb.com/) [`Minima-3.0`](https://github.com/jekyll/minima) theme with `solarized-dark` skin.


Install ruby 3.2.3 (it won't work with a more recent version).  The easiest way is to do this 
```bash
git clone https://github.com/rbenv/rbenv.git ~/.rbenv
~/.rbenv/bin/rbenv init
git clone https://github.com/rbenv/ruby-build.git "$(rbenv root)"/plugins/ruby-build
git -C "$(rbenv root)"/plugins/ruby-build pull
apt-get install autoconf patch build-essential rustc libssl-dev libyaml-dev libreadline6-dev zlib1g-dev libgmp-dev libncurses5-dev libffi-dev libgdbm6 libgdbm-dev libdb-dev uuid-dev
rbenv install 3.2.3 
```

which installs it via [ruby-build](https://github.com/rbenv/ruby-build), which is installed via [rbenv](https://github.com/rbenv/rbenv).  Then download this repository, change into it, run 
```bash 
bundle install
bundle exec jekyll serve
```
and it will update the html in real time as you changes of markdown files etc while serving the site to localhost.   