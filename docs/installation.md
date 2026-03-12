---
layout: default
title: Installation
nav_order: 3
---

# Installation

Follow these steps to run the documentation site locally on your machine.

---

## Step 1 – Clone the Repository

```bash
git clone https://github.com/MariekeVDA/MariekeVDA.github.io.git
cd MariekeVDA.github.io
```

---

## Step 2 – Install Ruby and Bundler

GitHub Pages uses Jekyll, which requires Ruby. Install it with your system's package manager:

**macOS (Homebrew)**
```bash
brew install ruby
gem install bundler
```

**Ubuntu / Debian**
```bash
sudo apt-get install ruby-full build-essential
gem install bundler
```

**Windows**
Download and install Ruby from [rubyinstaller.org](https://rubyinstaller.org/).

---

## Step 3 – Install Dependencies

Create a `Gemfile` (if one does not exist) with:

```ruby
source "https://rubygems.org"
gem "github-pages", group: :jekyll_plugins
```

Then run:

```bash
bundle install
```

---

## Step 4 – Serve the Site Locally

```bash
bundle exec jekyll serve
```

Open your browser and go to **http://localhost:4000**. The site will automatically reload when you save changes.

---

## Deploying to GitHub Pages

Just push your changes to the `main` branch:

```bash
git add .
git commit -m "Update documentation"
git push origin main
```

GitHub Pages will build and publish your site automatically within a minute or two.

---

[← Getting Started](getting-started) &nbsp;|&nbsp; [Usage →](usage)
