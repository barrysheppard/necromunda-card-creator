# Necromunda Card Creator

Using this is simple enough:

Type in the name of the card in the Card name section, add the card body text in the Body Text section, and type the card type in the footer.
All the texts will centre align.
The body text will attempt to carriage turn text that runs on, but you can also force returns by adding them in.
If you start body text with ** then that line will be in red and bold.
A number of logos are also available which if selected will appear in a faded red in the bottom corner.
Cards can be downloaded as a png by pressing 'Save card as image'.
Cards an be saved as a json file by pressing 'Save card as file', you can then later upload the json file using the choose file button. This can be handy if you type up a card and then notice a typo later.
Reset All will nuke everything back to default entries.
If you need the card back, you can find it here.
If you have any problems or have any suggestions please contact barrysheppard@gmail.com

This is a heavily hacked version of the [Warcry card generator](https://barrysheppard.github.io/warcry-card-creator/index.html) which in turn is a fork of [Hennirocks version](https://hennirocks.github.io/warcry-card-creator/) which was fork of [@rachelnertia's work](https://rachelnertia.github.io/warcry-card-creator/).

# Setting Up Local Development on macOS

This project uses HTML, CSS, and JavaScript to build a static web application for creating Necromunda cards. It leverages the Liquid templating syntax (such as {% include %}) to modularize HTML content and simplify site structure. The project is designed to be run locally or deployed as a static site, with assets and templates organized for easy customization and extension.

Follow these steps to set up Jekyll for local development:

## 1. Install Homebrew (if not already installed)

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

## 2. Install Ruby (recommended for Jekyll)

```sh
brew install ruby
```

## 3. Add Ruby to Your PATH

Add the following line to your `~/.bash_profile` or `~/.zshrc`:

```sh
echo 'export PATH="$HOME/.gem/ruby/3.4.0/bin:$PATH"' >> ~/.bash_profile
```

Then reload your shell:

```sh
source ~/.zshrc   # or source ~/.bash_profile
```

## 4. Install Jekyll and Bundler

```sh
gem install --user-install bundler jekyll
```

## 5. Create a Gemfile

```sh
bundle init
```

## 6. Edit the Gemfile - adding this line

```sh
gem "jekyll"
```

## 7. Install Dependencies

```sh
bundle install
```

## 8. Start the Jekyll Server

```sh
jekyll serve
```

## 9. Visit Your Site

Open the server address provided by Jekyll in your terminal.

---

### Notes

- Jekyll automatically processes `{% include %}` tags and front matter.
- Place your includes in the `_includes` directory.
- If you have a `_config.yml` file, Jekyll will use it for configuration.

---