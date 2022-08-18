---
title: How to setup Obisidan with GitHub                    # Add title of the machine here
date: 2022-08-18 08:00:00 -0600                           # Change the date to match completion date
categories: [Tips & Tricks]                     # Categories
tags: [github, blog, vscode, obsidian, pkm]     # TAG names should always be lowercase; add relevant tags
show_image_post: true                           # Change this to true
image: ../../assets/img/zweilosec-whoami.png         # Add image here for post preview image
---

My goal are to write blog post with the tool Obsidian in markdown and host them at Github with the Jekyll Chirpy theme.

### The Chirpy theme

![Screenshot of my Chirpy-themed website](../../assets/img/xyz.png)


### Ruby

The following must be installed first:

* Ruby version 2.5.0 or higher, including all development headers (check your Ruby version using `ruby -v`)
```bash
sudo apt install ruby-full build-essential zlib1g-dev
```
* RubyGems (should be included with Ruby, check your Gems version using `gem -v`)
* GCC and Make (should be included in your linux distro, check versions using `gcc -v`,`g++ -v`, and `make -v`)

Next, add the requisite lines to your `.bashrc` file by running each command below:

```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

### Jekyll

Next, install Jekyll and Bundler

```
gem install jekyll bundler
```

#### Blog Migrations