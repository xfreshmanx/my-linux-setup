# My Linux machine setup

> A List of applications and tools installed on my Linux Machine. This is inspired by nikitavoloboev´s [my-mac-os](https://github.com/nikitavoloboev/my-mac-os), but for Linux Based Systems.

For an automated provision scripts, powered by Ansible, please check the [provision](provision) folder.

## Motivation

Setup a new machine from scratch is always a very time consuming task. Last time I did it I took an entire weekend to install everything. And there is a high change of forget some less used command line tool. Also as the Developer I install many tools directly from GitHub and so checking if they are updated is a very manual process, like going to GitHub, check latest release, download the binary and move it to the correct place.

What if most of that, can be automated?

That´s what this repository does. In this README file you will encounter a list of software I use and can be seen as a reference. The more interesting part is in 
[provision](provision) folder, which contains a set of Ansible playbooks to automatically install that softtware.

As a Developer I need my main OS to be very stable but I also want to have regularly updated packages. After working with Debian based OSes for many years, in 2019 I decided to give a try to [Fedora](https://getfedora.org/) and so this playbook is optimized for Fedora.

## Table of Contents

- [My Linux machine setup](#my-linux-machine-setup)
  - [Motivation](#motivation)
  - [Table of Contents](#table-of-contents)
  - [Graphical Applications](#graphical-applications)
    - [Productivity](#productivity)
    - [Internet](#internet)
    - [Communication Tools](#communication-tools)
    - [Graphics & Design](#graphics--design)
    - [Sound & Video](#sound--video)
    - [Development Tools](#development-tools)
    - [Utilities](#utilities)
    - [Games](#games)
    - [Themes and Icons](#themes-and-icons)
    - [Fonts](#fonts)
  - [Terminal Applications](#terminal-applications)
    - [Shell configuration](#shell-configuration)
    - [File Navigation and Search](#file-navigation-and-search)
    - [Text Mainuplation](#text-mainuplation)
    - [Multimedia](#multimedia)
    - [Networking](#networking)
    - [Http Tools](#http-tools)
    - [Package Managers](#package-managers)
    - [Version Control](#version-control)
    - [Project Scaffolding](#project-scaffolding)
    - [Snippets and Cheat sheets](#snippets-and-cheat-sheets)
    - [Cloud clients](#cloud-clients)
    - [Docker Tools](#docker-tools)
  - [Infrastucture As Code](#infrastucture-as-code)
    - [Security](#security)
    - [System Utils](#system-utils)
    - [Other](#other)
  - [Development Runtimes](#development-runtimes)
  - [Other](#other-1)
    - [Gnome Extensions](#gnome-extensions)
    - [VS Code Extensions](#vs-code-extensions)
  - [Chrome Extensions](#chrome-extensions)

## Graphical Applications

In this section will be listed all the Graphical Applications. A separate section with Terminal applications after.

### Productivity

* [Libreoffice](https://libreoffice.org) - Office suite.
* [Gnome Calendar](https://wiki.gnome.org/Apps/Calendar) - Calendar application for GNOME
* [Gnome Contacts](https://wiki.gnome.org/Apps/Contacts) - Easy access to my Contacts List, syncted with Google Contacts.
* [Marker](https://flathub.org/apps/details/com.github.fabiocolacio.marker) - Powerfull Markdown editor.
* [Master PDF Editor](https://code-industry.net/masterpdfeditor/) - Edit text and images in PDF files
* [OpenPaper.work](https://openpaper.work/en-us/) -  Paperwork - Document management made fast and eas
* [Planner](https://flathub.org/apps/details/com.github.alainm23.planner) - Native TODO list application.
* [Foliate](https://flathub.org/apps/details/com.github.johnfactotum.Foliate) - Epub Reader
* [Notion (Web App)](https://www.notion.so) - My personal Knowledge base and notes application. Powered by [Nativefier](https://github.com/jiahaog/nativefier)
* [TickTick (Web App)](https://www.ticktick.com) - Todo list and reminders app. Powered by [Nativefier](https://github.com/jiahaog/nativefier)

### Internet

* [Firefox](https://www.mozilla.org/pt-PT/firefox/) - My primary browser
* [Google Chrome](https://www.google.com/chrome/) - My secondary browser
* [Dropbox](https://www.dropbox.com/home#/) - Easly share files between computers.
* [Transmission](https://transmissionbt.com/) - Torrent client
* [uget](https://ugetdm.com/) - Download manager
* [pennywise](https://github.com/kamranahmedse/pennywise) -  Cross-platform application to open any website or media in a floating window
* [Gufw Firewall](http://gufw.org/) - Gui for ufw, Uncomplicated Firewall.
* [Remmina](https://remmina.org/) - A feature rich Remote Desktop Application.

### Communication Tools

* [Skype](https://www.skype.com/) - Official Skype Application.
* [Slack](https://slack.com) - Official Slack application.
* [Polari](https://wiki.gnome.org/Apps/Polari) - Gnome IRC client.
* [Discord](https://discordapp.com/) - Free Voice and Text Chat for Gamers
* [Caprine](https://github.com/sindresorhus/caprine) - Elegant Facebook Messenger desktop app

### Graphics & Design

* [GIMP](https://www.gimp.org/) - GNU Image Manipulation Program
* [figma-linux](https://github.com/ChugunovRoman/figma-linux) - Figma is the first interface design tool based in the browser, making it easier for teams to create software
* [Flameshot](https://github.com/lupoDharkael/flameshot) - Powerful yet simple to use screenshot software with annotation support and easy upload to Imgur.
* [Peek](https://github.com/phw/peek) - Simple animated GIF screen recorder with an easy to use interface
* [Image Optimizer](https://flathub.org/apps/details/com.github.gijsgoudzwaard.image-optimizer) - Simple lossless image compression.
* [XnConvert](https://www.xnview.com/en/xnconvert/) - Batch Image Processing, Image Convertor, Image Resizer
* [drawio-desktop](https://github.com/jgraph/drawio-desktop) - Official electron build of draw.io
* [WireframeSketcher](https://wireframesketcher.com/) - Wireframing Tool for Professionals
* [Graphviz](https://www.graphviz.org/) - Graph Visualization Software
* [Inkscape](https://inkscape.org/) - Design tool
* [Avvie](https://flathub.org/apps/details/com.github.taiko2k.avvie) - A simple tool cropping and downsizing images. Suitable for avatars or cropping photos for use as desktop wallpapers. Convert PNG to JPG. Export in one click to your Pictures folder.
  
### Sound & Video

* [Spotify](https://www.spotify.com/) - Music for everyone.
* [Kdenlive](http://www.kdenlive.org/) - Video editor
* [Kazam](https://launchpad.net/kazam) - Screentast tool for linux
* [VLC](http://www.videolan.org/vlc/) - Media player
* [EasyTag](https://wiki.gnome.org/Apps/EasyTAG) - Audio file metadata editor
* [Audacity](https://sourceforge.net/projects/audacity/) - Audio editor
* [Lollypop](https://wiki.gnome.org/Apps/Lollypop) - Lollypop is a modern music player for GNOME.
* [FFaudioConverter](https://flathub.org/apps/details/com.github.Bleuzen.FFaudioConverter) - Convert music files between multiple formats
* [Gnome Podcasts](https://wiki.gnome.org/Apps/Podcasts) - Listen to your favorite podcasts.
* [Headset](https://headsetapp.co/) - Desktop Music Player Built on YouTube And Reddit.
* [youtube-dl-gui](https://github.com/MrS0m30n3/youtube-dl-gui) - A cross platform front\-end GUI of the popular youtube-dl.
* [Shortwave](https://flathub.org/apps/details/de.haeckerfelix.Shortwave) - Shortwave is an internet radio player that provides access to a station database with over 25,000 stations.
* [obs](https://obsproject.com/download) - Open Broadcaster Software.

### Development Tools

* [JetBrains Toolbox App](https://www.jetbrains.com/toolbox/app/) -  Manage Your Jetbrains Tools with Ease.
    * [PHPStorm](https://www.jetbrains.com/phpstorm/) - The Best PHP IDE by Jetbrains.
    * [Intelij](https://www.jetbrains.com/idea/) - Java and Android IDE.
    * [WebStorm](https://www.jetbrains.com/webstorm/) - General purpose Web IDE.
    * [GoLand](https://www.jetbrains.com/go/) - GoLand is a cross-platform IDE built specially for Go developers
* [Visual Studio Code](https://code.visualstudio.com/) - My text editor of choice
* [Cacher](https://www.cacher.io/) - Code snippet organizer for pros
* [Meld](http://meldmerge.org/) - Meld is a visual diff and merge tool targeted at developers
* [GitKraken](https://www.gitkraken.com/) - The legendary Git GUI client for Windows, Mac and Linux.
* [virt-manager](https://virt-manager.org/) - The virt-manager application is a desktop user interface for managing virtual machines through libvirt. It primarily targets KVM VMs, but also manages Xen and LXC (linux containers)
* [Postman](https://www.getpostman.com/) - Rest API Client
* [Regex Tester](https://flathub.org/apps/details/com.github.artemanufrij.regextester) - A simple app for testing regular expressions.
* [Glade](https://glade.gnome.org/) -  A User Interface Designer for Gnome based applications.
* [DBeaver](https://flathub.org/apps/details/io.dbeaver.DBeaverCommunity) - Universal Database Manager
* [Kubernetic](https://kubernetic.com/) - The Kubernetes Desktop Client
* [Spotlight studio](https://stoplight.io/) - The API Design Management Platform powering the world's leading API first companies.

### Utilities

* [Ulauncher](https://ulauncher.io/) - Application Launcher for Linux. A Linux alternative to [Alfted](https://www.alfredapp.com/)
* [Tilix](https://github.com/gnunn1/tilix) - A tiling terminal emulator for Linux using GTK+ 3
* [Bleachbit](https://www.bleachbit.org/) - System cleaner tool
* [Menulibre](https://launchpad.net/menulibre) - Menu editor
* [Stacer](https://github.com/oguzhaninan/Stacer) - Linux System Optimizer and Monitoring
* [GParted](https://gparted.sourceforge.io/) - GParted is a free partition editor for graphically managing your disk partitions
* [Restic](https://restic.net/) - Automatic and continuous backup to the cloud.
* [Font Finder](https://flathub.org/apps/details/io.github.mmstick.FontFinder) - An application for browsing and installing fonts from Google's font archive from the comfort of your Linux desktop.
* [Cryptomator](https://cryptomator.org/) - Free client-side encryption for your cloud files.
* [Grsync](https://sourceforge.net/projects/grsync/) - Grsync is used to synchronize folders, files and make backups. It is a rsync GUI (Graphical User Interface).
* [Etcher](https://www.balena.io/etcher/) - Flash OS images to SD cards & USB drives, safely and easily.

### Games

* [Steam](https://store.steampowered.com)
* [Gens/GS - Sega Retro](https://segaretro.org/Gens/GS)
* [Mines](https://wiki.gnome.org/Apps/Mines)

### Themes and Icons

* [nana-4/materia-theme](https://github.com/nana-4/materia-theme) - A Material Design theme for GNOME/GTK+ based desktop environments
* [arc-theme](https://github.com/horst3180/arc-theme) -  A flat theme with transparent elements.
* [papirus-icon-theme](https://github.com/PapirusDevelopmentTeam/papirus-icon-theme) - Papirus icon theme for Linux.

### Fonts

* [tonsky/FiraCode](https://github.com/tonsky/FiraCode) - Monospaced font with programming ligatures
* [i-tu/Hasklig: Hasklig](https://github.com/i-tu/Hasklig) - A code font with monospaced ligatures
* [Jetbrains Mono](https://www.jetbrains.com/lp/mono/) - A typeface for developers. By Jetbrains.

---

## Terminal Applications

A big part of my Development life is spent on the Terminal, so having a good set of tools there is essential.

### Shell configuration

I use ZSH shell with the following extras:

* [zplug](https://github.com/zplug/zplug) - A next-generation plugin manager for zsh
* [zsh-completions](https://github.com/zsh-users/zsh-completions) - Additional completion definitions for Zsh.
* [zsh-you-should-use](https://github.com/MichaelAquilina/zsh-you-should-use) - ZSH plugin that reminds you to use existing aliases for commands you just typed
* [zsh-history-substring-search](https://github.com/zsh-users/zsh-history-substring-search) - ZSH port of Fish history search (up arrow)
* [zsh-completions](https://github.com/zsh-users/zsh-completions) -  Additional completion definitions for Zsh.
* [zsh-autosuggestions](https://github.com/zsh-users/zsh-autosuggestions) -  Fish-like autosuggestions for Zsh.
* [powerlevel10k](https://github.com/romkatv/powerlevel10k) - A fast reimplementation of Powerlevel9k ZSH theme
* [powerline-fonts](https://github.com/powerline/fonts) - Patched fonts for Powerline users.

### File Navigation and Search

* [urbainvaes/fzf-marks](https://github.com/urbainvaes/fzf-marks) - Plugin to manage bookmarks in bash and zsh
* [agkozak/zsh-z](https://github.com/agkozak/zsh-z) - Jump quickly to directories that you have visited "frecently". A native ZSH port of z.
* [ranger](https://github.com/ranger/ranger) - A VIM-inspired filemanager for the console.
* [junegunn/fzf](https://github.com/junegunn/fzf) -  A command-line fuzzy finder
* [facebook/PathPicker](https://github.com/facebook/pathpicker/) - PathPicker accepts a wide range of input/output from git commands, grep results, searches pretty much anything.After parsing the input, PathPicker presents you with a nice UI to select which files you're interested in. After that you can open them in your favorite editor or execute arbitrary commands.
* [fd](https://github.com/sharkdp/fd) - A simple, fast and user-friendly alternative to 'find'
* [ripgrep](https://github.com/BurntSushi/ripgrep) - ripgrep recursively searches directories for a regex pattern.
* [sd](https://github.com/chmln/sd) - Intuitive find & replace CLI (sed alternative

### Text Mainuplation

* [vim](https://vim.org) with [vim-plug](https://github.com/junegunn/vim-plug) - Terminal based text editor.
* [bat](https://github.com/sharkdp/bat) - A cat(1) clone with wings. 
* [jq](https://github.com/stedolan/jq) - Command-line JSON processor.
* [fx](https://github.com/antonmedv/fx) - Command-line tool and terminal JSON viewer.
* [yq](https://github.com/mikefarah/yq) -  yq is a portable command-line YAML processor.
* [markdown-toc](https://github.com/jonschlinkert/markdown-toc) - Generate a markdown TOC (table of contents) for a README or any markdown files, using remgearkable.
* [tablemark-cli](https://github.com/citycide/tablemark-cli) - Generate markdown tables from JSON data at the command line.
* [pandoc](https://github.com/jgm/pandoc) - Universal markup converter
* [parse-columns-cli](https://github.com/sindresorhus/parse-columns-cli) - Parse text columns, like the output of unix commands. Returns JSON that you can manipulate with tools like jq or underscore-cli.
* [mdless](https://github.com/MikeyBurkman/mdless) -  Markdown Viewer for the CLI with highlighting and paging
* [lnav](http://lnav.org/) - The Log File Navigator
* [hasha-cli](https://github.com/sindrehasha-clisorhus/hasha-cli) - hashing made simple. Get the hash of text or stdin.

### Multimedia

* [jarun/imgp](https://github.com/jarun/imgp) - Multi-core batch image resizer and rotator
* [svg/svgo](https://github.com/svg/svgo) - Node.js tool for optimizing SVG files
* [youtube-dl](https://github.com/rg3/youtube-dl) - Command-line program to download videos from YouTube.com and other video sites
* [asciinema](https://asciinema.org/) - Record and share your terminal sessions, the right way
* [svg-term-cli](https://github.com/marionebl/svg-term-cli) - Share terminal sessions via SVG and CSS]

### Networking

- Netstat
- iotop
- nmap
* [get-port-cli](https://github.com/sindresorhus/get-port-cli) - Get an available port

### Http Tools

* [httpie](https://github.com/jakubroztocil/httpie) - Modern command line HTTP client – user-friendly curl alternative with intuitive UI, JSON support, syntax highlighting, wget-like downloads, extensions, etc
* [Artillery](https://artillery.io/) - A modern load testing toolkit
* [wg/wrk](https://github.com/wg/wrk) - Modern HTTP benchmarking tool

### Package Managers

* [composer](https://getcomposer.org/) - Dependency Manager for PHP
* [Yarn](https://yarnpkg.com/en/) - Modern Javascript Package manager.
* [cargo](https://crates.io/) -  Rust Package Registry

### Version Control

* [hub](https://github.com/github/hub) - hub helps you win at git.
* [lab](https://github.com/zaquestion/lab) - Lab wraps Git or Hub, making it simple to clone, fork, and interact with repositories on GitLab
* [tig](https://github.com/jonas/tig) - Text-mode interface for git
* [git-semver](https://github.com/ziishaned/git-semver) - A CLI tool to generate semver compliant tags for your git repositories 
* [git-extras](https://github.com/tj/git-extras) - GIT utilities, repo summary, repl, changelog population, author commit percentages and more
* [arc90/git-sweep](https://github.com/arc90/git-sweep) - : A command-line tool that helps you clean up Git branches that have been merged into master.
* [conventional-changelog](https://github.com/conventional-changelog/conventional-changelog/tree/master/packages/conventional-changelog-cli#readme)
* [commitizen/cz-cli](https://github.com/commitizen/cz-cli) - The commitizen command line utility.
* [semantic-release](https://github.com/semantic-release/semantic-release) - Fully automated version management and package publishing.
* [goreleaser/goreleaser](https://github.com/goreleaser/goreleaser) - Deliver Go binaries as fast and easily as possible.
* [cezaraugusto/mklicense](https://github.com/cezaraugusto/mklicense) -  CLI tool for generating Licenses\. Easily\.
* [TejasQ/add-gitignore](https://github.com/TejasQ/add-gitignore) -  An interactive CLI tool that adds a .gitignore to your projects.

### Project Scaffolding

* [saojs/sao](https://github.com/saojs/sao) - : Futuristic scaffolding tool.
* [hugo](https://github.com/gohugoio/hugo) - The world’s fastest framework for building websites.
* [Vue CLI 3](https://cli.vuejs.org/) - Standard Tooling for Vue.js Development.
* [vuejs/vuepress](https://github.com/vuejs/vuepress) - Minimalistic Vue-powered static site generator
* [@gridsome/cli](https://www.npmjs.com/package/@gridsome/cli) - A command line tool for creating new Gridsome projects.
* [Symfony CLI](https://symfony.com/download) - Symfony command line tool
* [serverless/serverless](https://github.com/serverless/serverless) - Serverless Framework – Build web, mobile and IoT applications with serverless architectures using AWS Lambda, Azure Functions, Google CloudFunctions & more!
* [gatsby-cli](https://www.npmjs.com/package/gatsby-cli) - The Gatsby command line interface (CLI). It is used to perform common functionality, such as creating a Gatsby application based on a starter, spinning up a hot-reloading local development server, and more!
* [readme-md-generator](https://github.com/kefranabg/readme-md-generator) - CLI that generates beautiful README.md files]
  
### Snippets and Cheat sheets

* [cacher-cli](https://github.com/CacherApp/cacher-cli) - The command line interface to Cacher.
* [tldr](https://github.com/tldr-pages/tldr) - Simplified and community\-driven man pages.
* [snipline](https://snipline.io/) - Command-line snippet organizer for power users.
* [santinic/how2](https://github.com/santinic/how2) - stackoverflow from the terminal
* [sgentle/caniuse-cmd](https://github.com/sgentle/caniuse-cmd) - Caniuse command line tool.

### Cloud clients

* [doctl](https://github.com/digitalocean/doctl) - A command line tool for DigitalOcean services.
* [Google Cloud SDK](https://cloud.google.com/sdk/gcloud/) - Google Cloud SDK.
* [AWS CLI](https://aws.amazon.com/cli) - AWS Command Line Interface.
* [Netlify Command Line Tools](https://www.netlify.com/docs/cli/) - Netlify’s command line tools let you deploy sites or configure continuous deployment straight from the command line.
* [The Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) - The Heroku Command Line Interface (CLI) makes it easy to create and manage your Heroku apps directly from the terminal. It’s an essential part of using Heroku.
* [cloudflare-cli](https://github.com/danielpigott/cloudflare-cli) - CLI for interacting with Cloudflare
* [firebase-tools](https://firebase.google.com/docs/cli) - Firebase Command Line tools
* [fauna/fauna-shell](https://github.com/fauna/fauna-shell) - Interactive shell for FaunaDB

### Docker Tools

* [docker-compose](https://github.com/docker/compose) - Define and run multi-container applications with Docker
* [ctop](https://github.com/bcicen/ctop) - Top-like interface for container metrics
* [dive](https://github.com/wagoodman/dive) - A tool for exploring each layer in a docker image
* [stern](https://github.com/wercker/stern) - Multi pod and container log tailing for Kubernetes
* [lazydocker](https://github.com/jesseduffield/lazydocker) - The lazier way to manage everything docker
* [minikube](https://github.com/kubernetes/minikube) - Run Kubernetes locally
* [kubectl](https://github.com/kubernetes/kubernetes/tree/master/pkg/kubectl) - Kubernetes Control
* [kubectx](https://github.com/ahmetb/kubectx) - Fast way to switch between clusters and namespaces in kubectl
* [k9s](https://github.com/derailed/k9s) - Kubernetes CLI To Manage Your Clusters In Style!
* [fluxctl](https://github.com/fluxcd/flux) - Flux Command line tool.
* [helm](https://helm.sh/) - The package manager for Kubernetes.
* [kubeval](https://github.com/instrumenta/kubeval) - Validate your Kubernetes configuration files, supports multiple Kubernetes versions
* [kubeseal](https://github.com/bitnami-labs/sealed-secrets) - CLI tool for encrypt and decrypt Bitnani sealed secrets
* [open-policy-agent/conftest](https://github.com/open-policy-agent/conftest) - Write tests against structured configuration data using the Open Policy Agent Rego query language

## Infrastucture As Code.

* [Terraform](https://www.terraform.io/) - Write, Plan, and Create Infrastructure as Code.
* [Ansible](https://www.ansible.com/) - Simple, agentless IT automation that anyone can use.
  * [ansible/ansible-lint](https://github.com/ansible/ansible-lint) - Best practices checker for Ansible
  * [Ansible Galaxy](https://galaxy.ansible.com/) - Jump-start your automation project with great content from the Ansible community. Galaxy provides pre-packaged units of work known to Ansible as roles.
* [Pulumi](https://www.pulumi.com/) -  Modern Infrastructure as Code
* [terratest](https://github.com/gruntwork-io/terratest/releases) - Terratest is a Go library that makes it easier to write automated tests for your infrastructure code. 

### Security

* [pwgen](https://linux.die.net/man/1/pwgen) - make pronounceable passwords.
* [lastpass-cli](https://github.com/lastpass/lastpass-cli) - LastPass command line interface tool

### System Utils

* [htop](https://github.com/hishamhm/htop) - htop is an interactive text-mode process viewer for Unix systems.
* [fkill-cli](https://github.com/sindresorhus/fkill-cli) - Fabulously kill processes. Cross-platform.
* [trash-cli](https://github.com/sindresorhus/trash-cli) - Move files and folders to the trash.
* [tmux](https://github.com/tmux/tmux) and [tmuxp](https://github.com/tmux-python/tmuxp) - Terminal multiplexer and session manager.
* [yadm](https://github.com/TheLocehiliosan/yadm) - yadm is a tool for managing dotfiles.
* [direnv](https://direnv.net/) - direnv is an extension for your shell. It augments existing shells with a new feature that can load and unload environment variables depending on the current directory.
* [ncdu](https://linux.die.net/man/1/ncdu) - Disk usage visualization from terminal.
* [glances](https://github.com/nicolargo/glances) - Glances an Eye on your system. A top/htop alternative for GNU/Linux, BSD, Mac OS and Windows operating systems.

### Other

* [localtunnel/localtunnel](https://github.com/localtunnel/localtunnel) - expose your machine to the world.
* [FiloSottile/mkcert: A simple zero-config tool to make locally trusted development certificates with any names you'd like.](https://github.com/FiloSottile/mkcert)
* [serverless/serverless](https://github.com/serverless/serverless)
* [mycli](https://www.mycli.net/) - MyCLI is a command line interface for MySQL, MariaDB, and Percona with auto-completion and syntax highlighting.
* [carbon-now-cli](https://github.com/mixn/carbon-now-cli) - Beautiful images of your code — from right inside your terminal.
* [figlet](http://www.figlet.org/) - FIGlet is a program for making large letters out of ordinary text
* [Teleconsole](https://www.teleconsole.com/) - your UNIX terminal in seconds!
* [sitespeed.io](https://github.com/sitespeedio/sitespeed.io) - Open source tool that helps you monitor, analyze and optimize your website speed and performance, based on performance best practices advices.
* [mermaid.cli](https://github.com/mermaidjs/mermaid.cli) - Generate Diagrams using Mermaid.
* [Devilspie2](http://www.nongnu.org/devilspie2/) - Devilspie2 is a window matching utility, allowing the user to perform scripted actions on windows as they are created. For example you can script a terminal program to always be positioned at a specific screen position, or position a window on a specific workspace
* [wmctrl](https://linux.die.net/man/1/wmctrl) - wmctrl is a command that can be used to interact with an X Window manager that is compatible with the EWMH/NetWM specification.

## Development Runtimes

* PHP
* NodeJS
* Golang
* Ruby
* Python
* Vala

---

## Other

### Gnome Extensions

* [Caffeine](https://extensions.gnome.org/extension/517/caffeine/) - Disable the screensaver and auto suspend
* [Clipboard Indicator](https://extensions.gnome.org/extension/779/clipboard-indicator/) - Clipboard Manager extension for Gnome-Shell - Adds a clipboard indicator to the top panel, and caches clipboard history.
* [Coverflow Alt-Tab](https://extensions.gnome.org/extension/97/coverflow-alt-tab/) - Replacement of Alt-Tab, iterates through windows in a cover-flow manner.
* [Emoji Selector](https://extensions.gnome.org/extension/1162/emoji-selector/) - This extension provides a parametrable popup menu displaying most emojis, clicking on an emoji copies it to the clipboard.
* [GSConnect](https://extensions.gnome.org/extension/1319/gsconnect/) - KDE Connect allows devices to securely share content like notifications or files and other features like SMS messaging and remote control.
* [Always Indicator](https://extensions.gnome.org/extension/2594/always-indicator/) - Always show the new messages indicator on new messages. Features: 1) New message indicator is always shown if there are notifications.
* [Time ++](https://extensions.gnome.org/extension/1238/time/) - A todo.txt manager, time tracker, timer, stopwatch, pomodoro, and alarm clock
* [Vitals](https://extensions.gnome.org/extension/1460/vitals/) - A glimpse into your computer's temperature, voltage, fan speed, memory usage, processor load, system resources, network speed and storage stats.
* [ShellTile](https://extensions.gnome.org/extension/657/shelltile/) - A tiling window extension for GNOME Shell. Just move a window to the edges of the screen to create a tiling, otherwise move a window over another one, holding down the Control key.
* [Auto Move Windows](https://extensions.gnome.org/extension/16/auto-move-windows/) - Move applications to specific workspaces when they create windows.
* [Status Area Horizontal Spacing](https://extensions.gnome.org/extension/355/status-area-horizontal-spacing/)
* [Cast to TV](https://extensions.gnome.org/extension/1544/cast-to-tv/) - Cast files to Chromecast, web browser or media player app over local network.
* [Laine](https://extensions.gnome.org/extension/937/laine/) - Volume control extension.
* [Argos](https://extensions.gnome.org/extension/1176/argos/) - Create GNOME Shell extensions in seconds.
    * [pionl/bitbar-gitlab-ci](https://github.com/pionl/bitbar-gitlab-ci) -  Shows currently running pipelines from your GitLab in your bar.
* [VSCode Search Provider](https://extensions.gnome.org/extension/1207/vscode-search-provider/) - Provide recent VSCode projects as search results in overview
  
### VS Code Extensions

* 42Crunch.vscode-openapi
* abusaidm.html-snippets
* adrianwilczynski.alpine-js-intellisense
* akamud.vscode-caniuse
* AlanWalk.markdown-toc
* alefragnani.project-manager
* andischerer.theme-atom-one-dark
* anseki.vscode-color
* ashinzekene.nestjs
* axetroy.vscode-comment-autocomplete
* bajdzis.vscode-twig-pack
* be5invis.toml
* benjaminromano.typings-installer
* bradlc.vscode-tailwindcss
* Cacher.cacher-vscode
* capaj.vscode-exports-autocomplete
* castwide.solargraph
* christian-kohler.npm-intellisense
* codezombiech.gitignore
* CoenraadS.bracket-pair-colorizer
* cssho.vscode-svgviewer
* dbaeumer.vscode-eslint
* dbankier.vscode-gist
* dinhani.divider
* donjayamanne.jquerysnippets
* DotJoshJohnson.xml
* eamodio.gitlens
* EditorConfig.EditorConfig
* eg2.vscode-npm-script
* emilast.LogFileHighlighter
* ericadamski.carbon-now-sh
* eriklynd.json-tools
* esbenp.prettier-vscode
* fatihacet.gitlab-workflow
* fauna.faunadb
* felixfbecker.php-debug
* gio00.css-inline
* haaaad.ansible
* idleberg.badges
* idleberg.icon-fonts
* ikappas.composer
* ipedrazas.kubernetes-snippets
* JakeWilson.vscode-placeholder-images
* jcmordan.mark-as-excluded
* jerriepelser.copy-markdown-as-html
* jgsqware.gitlab-ci-templates
* joelday.docthis
* johnpapa.vscode-peacock
* josa.markdown-table-formatter
* marclipovsky.string-manipulation
* MattiasPernhult.vscode-todo
* mauve.terraform
* michelemelluso.gitignore
* mikestead.dotenv
* milovidov.escape-quotes
* mindginative.terraform-snippets
* mohsen1.prettify-json
* mrmlnc.vscode-autoprefixer
* ms-azuretools.vscode-docker
* ms-kubernetes-tools.vscode-kubernetes-tools
* ms-python.python
* ms-vscode.Go
* msjsdiag.debugger-for-chrome
* nickdemayo.vscode-json-editor
* octref.vetur
* octref.vscode-json-transform
* Orta.vscode-jest
* qinjia.view-in-browser
* ragingwind.web-manifest-snippets
* rebornix.project-snippets
* rebornix.ruby
* redhat.vscode-yaml
* rpinski.shebang-snippets
* rubbersheep.gi
* ryanolsonx.snippet-creator
* ryu1kn.annotator
* Shan.code-settings-sync
* shanoor.vscode-nginx
* Sophisticode.php-formatter
* stylelint.vscode-stylelint
* teamchilla.blueprint
* thekalinga.bootstrap4-vscode
* thomas-baumgaertner.vcl
* Tyriar.lorem-ipsum
* ultram4rine.vscode-choosealicense
* vscoss.vscode-ansible
* whatwedo.twig
* wholroyd.jinja
* wingrunr21.vscode-ruby
* wix.vscode-import-cost
* wmontalvo.vsc-meta-snippet
* xyz.local-history
* yzhang.markdown-all-in-one
* zhuangtongfa.material-theme
* Zignd.html-css-class-completion

## Chrome Extensions

* 365Scores - Live Scores and Sports News
* Auto Replay for YouTube™
* Blackfire Companion
* Copycat
* Copyfish 🐟 Free OCR Software
* Create Link
* Docs
* DownAlbum
* EditThisCookie
* Export links of all extensions
* Feedly Subscribe Button
* GNOME Shell integration
* Google Docs Offline
* Google Drive
* Google Keep
* Google Maps
* Google Photos
* Grammarly for Chrome
* I don't care about cookies
* JetBrains Toolbox Extension
* JSON Editor Online
* JSON Formatter
* Kindle Cloud Reader
* LastPass: Free Password Manager
* Notion Web Clipper
* Omnibox for Github
* Photo Zoom for Facebook
* Picture-in-Picture Extension (by Google)
* Qlearly - Tab and Bookmark Manager
* Saka
* Save to Pocket
* SearchPreview
* Sheets
* Slides
* Speedtest by Ookla
* Split Tabs
* StackEdit
* Tab to Window/Popup - Keyboard Shortcut
* Trello
* TurboNote
* TweetDeck
* Twitter
* uBlock Origin
* Vue.js devtools
* Web Developer
* WhatFont
* Cacher
* Diigo Web Collector - Capture and Annotate
* imgur Uploader
* Linkclump
* Office Editing for Docs, Sheets & Slides
* Pinterest Save Button
* The Great Suspender
* Xdebug helper
