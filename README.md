# rails practice

## about

This repository is practice to develop rails application.

## setup

### install dependency modules

#### install brew packages

If you do not install brew, [see 'install brew' from this link](https://brew.sh/).

After installed brew, install package like this.

```bash
brew install libxml2 libxslt libiconv
```

#### install rbenv

If you do not install rbenv, exec commands like this.

```bash
brew install openssl readline rbenv ruby-build
echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
```

#### install node env

```bash
brew install ndenv node-build
echo 'export PATH="$HOME/.ndenv/bin:$PATH"' >> ~/.bash_profile
echo 'eval "$(ndenv init -)"' >> ~/.bash_profile
```

#### install ruby of version for this application

```bash
rbenv install $(cat .ruby-version)
ndenv install $(cat .node-version)
```

#### set up gems and node packacges

```bash
gem install bundler
bundle install --path vendor/bundle
npm install
bin/rails db:create
bin/rails db:migrate
```

if fail install at `bundle install`, may be not enough installed packages from brew. see error logs carefully and Search in Google.