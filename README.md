# richardm.github.io

The codebase for my personal website.

## CI / CD Notes

This static generated site is built with GitHub Actions and deployed via GitHub Pages. To avoid surprises in production, don't let your local dev envrionment get ahead of the latest GitHub Pages' [supported versions](https://pages.github.com/versions/) of Ruby and other dependencies.

As of June 2025:

- Ruby 3.3.4
- Jekyll 3.10.0
- github-pages 232

## Running this Jekyll site on MacOS

There are two key parts to this:

1. Setting up Ruby on the dev machine (ideally this would be a docker container)
2. Installing Jekyll and managing the project's dependencies (which are constrained by GitHub)

## Part 1: Setting up Ruby on dev machine

- The following comes from this guide: https://jekyllrb.com/docs/installation/macos/
- Avoid using the default installed MacOS version of Ruby, and instead use the following:

| Tool             | Purpose                                                       |
| ---------------- | ------------------------------------------------------------- |
| **ruby-install** | Use it to install different versions of Ruby onto your system |
| **chruby**       | Use it to switch between those installed Ruby versions        |

### Installing Ruby

1. Install Homebrew if not already installed
2. `brew install ruby-install`
3. `brew install chruby`
4. Install jekyll: `gem install jekyll`

### Updating Ruby

```
brew update
brew upgrade chruby
chruby --version
```

To install various versions of Ruby:

- Run `ruby-install ruby 3.3.4` (see below, don't get ahead of GitHub's supported version)
- Note: You will need to quit and restart your terminal (or open a new shell) before proceeding
- Run `chruby` to list your installed Ruby versions and see which version is being used
- Run `chruby 3.4.1` to switch to that version of Ruby

## Part 2: To run Jekyll locally after installing Ruby:

- Make sure you're using the expected version of Ruby
- Run `bundle install` to install your project's dependencies
- Then run `bundle exec jekyll serve --livereload`

### Managing dependencies:

- The project's Ruby dependencies are specified in Gemfile and Gemfile.lock (similar to npm's package.json and package-lock.json)
- Run `bundle install` to install your project's dependencies (it's like npm install)
- Run `bundle add webrick` to add a dependency named webrick to the project
