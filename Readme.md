# Zebin Ren's Website

## Building Locally

### Install (mac)

Install environments:

```bash
brew install chruby ruby-install xz
ruby-install ruby 3.1.3

# If using bash, replace .zshrc with .bash_profile
echo "source $(brew --prefix)/opt/chruby/share/chruby/chruby.sh" >> ~/.zshrc
echo "source $(brew --prefix)/opt/chruby/share/chruby/auto.sh" >> ~/.zshrc
echo "chruby ruby-3.1.3" >> ~/.zshrc # run 'chruby' to see actual version
source ~/.zshrc

# The following cmd should show ruby3.1.3
ruby -v

# Install gem
gem install jekyll
```

Build and serve the site:

```bash
bundle install
bundle exec jekyll serve
```

References:
* [Testing your GitHub Pages site locally with Jekyll](https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/testing-your-github-pages-site-locally-with-jekyll?platform=mac)
* [Jekyll on macOS](https://jekyllrb.com/docs/installation/macos/)