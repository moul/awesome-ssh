# Awesome SSH [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of _SSH_ [apps](#apps), [libraries](#libraries) and [resources](#resources).

<h2 align="center"><img src="https://raw.githubusercontent.com/moul/awesome-ssh/master/logo.jpg" width="400" /></h2>

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.

Please read the [contribution guidelines](CONTRIBUTING.md) if you want to contribute.

**Check out my [blog](https://manfred.life/) 🦄 or say _hi_ on [Twitter](https://twitter.com/moul).**

## Table of Contents

- [Apps](#apps)
  - [`.ssh/config`](#sshconfig)
  - [Tools using the _SSH_ protocol](#tools-using-the-ssh-protocol)
  - [Servers](#servers)
  - [Network](#network)
  - [Multiplexers](#multiplexers)
  - [SSH Keys / Authentication](#ssh-keys--authentication)
  - [SSH agent](#ssh-agent)
  - [Tools](#tools)
  - [Automation](#automation)
  - [Web](#web)
  - [Testing / Honeypots](#testing--honeypots)
  - [Alternatives to SSH](#alternatives-to-ssh)
- [Libraries](#libraries)
- [Resources](#resources)
  - [Tutorials](#tutorials)
  - [Security](#security)
  - [Documentation](#documentation)
  - [Community](#community)

## Apps

### `.ssh/config`

- [`assh`](https://github.com/moul/assh) [![stars](https://img.shields.io/github/stars/moul/advanced-ssh-config.svg?style=social&label=stars)](https://github.com/moul/advanced-ssh-config) - Transparent wrapper (ProxyCommand) that adds regex, aliases, gateways, includes, dynamic hostnames to _SSH_ and `ssh-config`. _Previously: `advanced-ssh-config`_
- [storm](https://github.com/emre/storm) [![stars](https://img.shields.io/github/stars/emre/storm.svg?style=social&label=stars)](https://github.com/emre/storm) - Manage your _SSH_ like a boss.
- [ansible-ssh-config](https://github.com/gaqzi/ansible-ssh-config) [![stars](https://img.shields.io/github/stars/gaqzi/ansible-ssh-config.svg?style=social&label=stars)](https://github.com/gaqzi/ansible-ssh-config) - Letting _Ansible_ manage `ssh_config`.
- [ec2ssh](https://github.com/mirakui/ec2ssh) [![stars](https://img.shields.io/github/stars/mirakui/ec2ssh.svg?style=social&label=stars)](https://github.com/mirakui/ec2ssh) - A `ssh_config` manager for _AWS EC2_.
- [ssh-config](https://github.com/dbrady/ssh-config) [![stars](https://img.shields.io/github/stars/dbrady/ssh-config.svg?style=social&label=stars)](https://github.com/dbrady/ssh-config) - A tool to help manage your `.ssh/config` file.

### Tools using the _SSH_ protocol

- [scp](http://linux.die.net/man/1/scp) - Secure remote file copy utility over _SSH_.
- [rsync](https://rsync.samba.org) - Fast incremental transfer utility that supports _SSH_.
- [sftp](https://en.wikipedia.org/wiki/SSH_File_Transfer_Protocol) - File transfer protocol over _SSH_.
- [curl](http://curl.haxx.se) - Command line tool and library to transfer data (support `sftp`).

### Servers

- [sshportal](https://github.com/moul/sshportal) [![stars](https://img.shields.io/github/stars/moul/sshportal.svg?style=social&label=stars)](https://github.com/moul/sshportal) - simple, fun, and transparent SSH (& Telnet) Bastion Server
- [ssh2docker](https://github.com/moul/ssh2docker) [![stars](https://img.shields.io/github/stars/moul/ssh2docker.svg?style=social&label=stars)](https://github.com/moul/ssh2docker) - _SSH_ server to Docker containers.
- [ssh-proxy](https://github.com/ml-tooling/ssh-proxy) [![stars](https://img.shields.io/github/stars/ml-tooling/ssh-proxy.svg?style=social&label=stars)](https://github.com/ml-tooling/ssh-proxy) - Dockerized SSH bastion to proxy SSH connections to arbitrary containers.
- [whosthere](https://github.com/FiloSottile/whosthere) [![stars](https://img.shields.io/github/stars/FiloSottile/whosthere.svg?style=social&label=stars)](https://github.com/FiloSottile/whosthere) - A _SSH_ server that knows who you are. `$ ssh whoami.filippo.io`.
- [sshfront](https://github.com/gliderlabs/sshfront) [![stars](https://img.shields.io/github/stars/gliderlabs/sshfront.svg?style=social&label=stars)](https://github.com/gliderlabs/sshfront) - Programmable _SSH_ frontend.
- [ssh-chat](https://github.com/shazow/ssh-chat) [![stars](https://img.shields.io/github/stars/shazow/ssh-chat.svg?style=social&label=stars)](https://github.com/shazow/ssh-chat) - Chat over _SSH_.
- [sshcommand](https://github.com/dokku/sshcommand) [![stars](https://img.shields.io/github/stars/dokku/sshcommand.svg?style=social&label=stars)](https://github.com/dokku/sshcommand) - Turn _SSH_ into a thin client specifically for your app.
- [sshmuxd](https://github.com/joushou/sshmuxd) [![stars](https://img.shields.io/github/stars/joushou/sshmuxd.svg?style=social&label=stars)](https://github.com/joushou/sshmuxd) - `sshmux` frontend.
- [x84](https://github.com/jquast/x84) [![stars](https://img.shields.io/github/stars/jquast/x84.svg?style=social&label=stars)](https://github.com/jquast/x84) - A _python_ `telnet`/`ssh` server for modern _UTF-8_ and classic _cp437_ network virtual terminals. In spirit of classic software such as _ami/x_, _teleguard_, _renegade_, _iniquity_.
- [teleport](https://github.com/gravitational/teleport) [![stars](https://img.shields.io/github/stars/gravitational/teleport.svg?style=social&label=stars)](https://github.com/gravitational/teleport) - Modern _SSH_ server for clusters and teams.
- [ShellHub](https://github.com/shellhub-io/shellhub) [![stars](https://img.shields.io/github/stars/shellhub-io/shellhub.svg?style=social&label=stars)](https://github.com/shellhub-io/shellhub) - A _SSH_ gateway for remotely accessing any Linux device behind firewall and NAT.

### Network

- [Mosh](https://mosh.mit.edu) - The mobile shell.
- [sshfs](https://github.com/libfuse/sshfs) [![stars](https://img.shields.io/github/stars/libfuse/sshfs.svg?style=social&label=stars)](https://github.com/libfuse/sshfs) - Filesystem client based on the _SSH_ File Transfer Protocol.
- [ngrok](https://github.com/inconshreveable/ngrok) [![stars](https://img.shields.io/github/stars/inconshreveable/ngrok.svg?style=social&label=stars)](https://github.com/inconshreveable/ngrok) - Introspected tunnels to localhost.
- [localtunnel](https://github.com/progrium/localtunnel) [![stars](https://img.shields.io/github/stars/progrium/localtunnel.svg?style=social&label=stars)](https://github.com/progrium/localtunnel) - Expose localhost servers to the Internet.
- [sshuttle](https://github.com/sshuttle/sshuttle) [![stars](https://img.shields.io/github/stars/sshuttle/sshuttle.svg?style=social&label=stars)](https://github.com/sshuttle/sshuttle) - Transparent proxy server that works as a poor man's _VPN_. Forwards over `ssh`. Doesn't require admin. Works with _Linux_ and _MacOS_. Supports _DNS tunneling_.
- [sshttp](https://github.com/stealth/sshttp) [![stars](https://img.shields.io/github/stars/stealth/sshttp.svg?style=social&label=stars)](https://github.com/stealth/sshttp) - _SSH_/_HTTP(S)_ multiplexer. Run a webserver and a `sshd` on the same port w/o changes.
- [switcher](https://github.com/jamescun/switcher) [![stars](https://img.shields.io/github/stars/jamescun/switcher.svg?style=social&label=stars)](https://github.com/jamescun/switcher) - Run _SSH_ and _HTTP(S)_ on the same port.
- [sslh](https://github.com/yrutschle/sslh) [![stars](https://img.shields.io/github/stars/yrutschle/sslh.svg?style=social&label=stars)](https://github.com/yrutschle/sslh) - Applicative Protocol Multiplexer (i.e: _SSH_ + _HTTPS_).
- [tund](https://github.com/aphyr/tund) [![stars](https://img.shields.io/github/stars/aphyr/tund.svg?style=social&label=stars)](https://github.com/aphyr/tund) - _SSH_ reverse tunnel daemon.
- [autossh](http://www.harding.motd.ca/autossh/) - Automatically respawn _SSH_ session after network interruption.
- [wssh](https://github.com/aluzzardi/wssh) [![stars](https://img.shields.io/github/stars/aluzzardi/wssh.svg?style=social&label=stars)](https://github.com/aluzzardi/wssh) - _SSH_ to WebSockets Bridge.
- [docker-volume-sshfs](https://github.com/vieux/docker-volume-sshfs) [![stars](https://img.shields.io/github/stars/vieux/docker-volume-sshfs.svg?style=social&label=stars)](https://github.com/vieux/docker-volume-sshfs) - `sshfs` docker volume plugin.
- [quicssh](https://github.com/moul/quicssh) [![stars](https://img.shields.io/github/stars/moul/quicssh.svg?style=social&label=stars)](https://github.com/moul/quicssh) - QUIC proxy for SSH
- [sshpiper](https://github.com/tg123/sshpiper) [![stars](https://img.shields.io/github/stars/tg123/sshpiper.svg?style=social&label=stars)](https://github.com/tg123/sshpiper) - The missing reverse proxy for ssh scp.
- [sshhub](https://sshhub.de) - Web Service: access your SSH servers behind firewalls (ssh-teamviewer).

### Multiplexers

- [tmux](https://tmux.github.io) - Terminal multiplexer.
- [clusterssh](https://github.com/duncs/clusterssh) [![stars](https://img.shields.io/github/stars/duncs/clusterssh.svg?style=social&label=stars)](https://github.com/duncs/clusterssh) - Cluster admin via _SSH_.
- [tmux-cssh](https://github.com/dennishafemann/tmux-cssh) [![stars](https://img.shields.io/github/stars/dennishafemann/tmux-cssh.svg?style=social&label=stars)](https://github.com/dennishafemann/tmux-cssh) - `tmux` with a _ClusterSSH_-like behavior.
- [tm](https://github.com/Ganneff/tm) [![stars](https://img.shields.io/github/stars/Ganneff/tm.svg?style=social&label=stars)](https://github.com/Ganneff/tm) - `tmux` manager / helper.
- [i2cssh](https://github.com/wouterdebie/i2cssh) [![stars](https://img.shields.io/github/stars/wouterdebie/i2cssh.svg?style=social&label=stars)](https://github.com/wouterdebie/i2cssh) - `csshX` like _SSH_ tool for _iTerm2_.
- [ClusterSSH](http://sourceforge.net/projects/clusterssh/) - Controls a number of `xterm` windows via a single graphical console.

### _SSH_ keys / Authentication

- [authy-ssh](https://github.com/authy/authy-ssh) [![stars](https://img.shields.io/github/stars/authy/authy-ssh.svg?style=social&label=stars)](https://github.com/authy/authy-ssh) - Easy _two-factor_ authentication for _SSH_ servers.
- [github-auth](https://github.com/chrishunt/github-auth) [![stars](https://img.shields.io/github/stars/chrishunt/github-auth.svg?style=social&label=stars)](https://github.com/chrishunt/github-auth) - _SSH_ key management for GitHub users.
- [cipherhub](https://github.com/substack/cipherhub) [![stars](https://img.shields.io/github/stars/substack/cipherhub.svg?style=social&label=stars)](https://github.com/substack/cipherhub) - Encrypt messages based on _SSH_ public keys with easy import from GitHub.
- [Slack notifications](http://www.ryanbrink.com/slack-ssh-session-notifications/) ([archived version](https://web.archive.org/web/20160505202303/http://www.ryanbrink.com/slack-ssh-session-notifications/)) - Guide to setup Slack notifications (can be modified for other services).
- [totp-ssh-fluxer](https://github.com/benjojo/totp-ssh-fluxer) [![stars](https://img.shields.io/github/stars/benjojo/totp-ssh-fluxer.svg?style=social&label=stars)](https://github.com/benjojo/totp-ssh-fluxer) - A way to make sure your `sshd` port changes every 30 seconds.
- [github-keygen](https://github.com/dolmen/github-keygen) [![stars](https://img.shields.io/github/stars/dolmen/github-keygen.svg?style=social&label=stars)](https://github.com/dolmen/github-keygen) - Easy creation of secure _SSH_ configuration for your GitHub account(s).
- [kr](https://github.com/KryptCo/kr) [![stars](https://img.shields.io/github/stars/dolmen/github-keygen.svg?style=social&label=stars)](https://github.com/KryptCo/kr) - Kr agent that route access request to the paired mobile phone where Kryptonite is installed.
- [ServerAuth](https://serverauth.com) - Automatically sync SSH access across servers
- [ssh-inscribe](https://github.com/aakso/ssh-inscribe) - SSH key certificate creation and management tools.

### _SSH_ agent

- [ssh-ident](https://github.com/ccontavalli/ssh-ident) [![stars](https://img.shields.io/github/stars/ccontavalli/ssh-ident.svg?style=social&label=stars)](https://github.com/ccontavalli/ssh-ident) - Different agents and different keys for different projects, with `ssh`.
- [oh-my-zsh/plugins/ssh-agent](https://github.com/robbyrussell/oh-my-zsh) [![stars](https://img.shields.io/github/stars/robbyrussell/oh-my-zsh.svg?style=social&label=stars)](https://github.com/robbyrussell/oh-my-zsh) - `ssh-agent` plugin for `zsh`.
- [sshecret](https://github.com/thcipriani/sshecret) - Automatically create and manage multiple agents for multiple keys.

### Tools

- [sshrc](https://github.com/danrabinowitz/sshrc) [![stars](https://img.shields.io/github/stars/danrabinowitz/sshrc.svg?style=social&label=stars)](https://github.com/danrabinowitz/sshrc) - Bring your `.bashrc`, `.vimrc`, etc. with you when you `ssh`.
- [kyrat](https://github.com/fsquillace/kyrat) [![stars](https://img.shields.io/github/stars/fsquillace/kyrat.svg?style=social&label=stars)](https://github.com/fsquillace/kyrat) - SSH wrapper script that brings your dotfiles always with you on Linux and OSX.
- [ssh-vault](https://github.com/ssh-vault/ssh-vault) [![stars](https://img.shields.io/github/stars/ssh-vault/ssh-vault.svg?style=social&label=stars)](https://github.com/ssh-vault/ssh-vault) - encrypt/decrypt files using ssh keys
- [ssh-ping](https://github.com/vaporup/ssh-tools) [![stars](https://img.shields.io/github/stars/vaporup/ssh-tools.svg?style=social&label=stars)](https://github.com/vaporup/ssh-tools) - check if host is reachable using ssh_config
- [SSHPry v2](https://github.com/nopernik/SSHPry2.0) [![stars](https://img.shields.io/github/stars/nopernik/SSHPry2.0.svg?style=social&label=stars)](https://github.com/nopernik/SSHPry2.0) - Spy & Control os SSH Connected client's TTY
- [redial](https://github.com/taypo/redial) [![stars](https://img.shields.io/github/stars/taypo/redial?style=social)](https://github.com/taypo/redial) - Terminal Based SSH Session Manager for Unix Systems

### Automation

- [Ansible](https://github.com/ansible/ansible) [![stars](https://img.shields.io/github/stars/ansible/ansible.svg?style=social&label=stars)](https://github.com/ansible/ansible) - App deployment, configuration management and orchestration over _SSH_.
- [rtop](https://github.com/rapidloop/rtop) [![stars](https://img.shields.io/github/stars/rapidloop/rtop.svg?style=social&label=stars)](https://github.com/rapidloop/rtop) - Interactive, remote system monitoring tool based on _SSH_.
- [DSH - Dancer's shell / distributed shell](https://www.netfort.gr.jp/~dancer/software/dsh.html.en) - Wrapper for executing multiple remote shell commands from one command line.
- [parallel-ssh](https://github.com/ParallelSSH/parallel-ssh) [![stars](https://img.shields.io/github/stars/ParallelSSH/parallel-ssh.svg?style=social&label=stars)](https://github.com/ParallelSSH/parallel-ssh) - Provides parallel versions of OpenSSH and related tools.
- [SSH Power Tool](https://code.google.com/p/sshpt/) - Execute commands and upload files to many servers simultaneously without using pre-shared keys.

### Web

- [Secure Shell chrome extension](https://chrome.google.com/webstore/detail/secure-shell/pnhechapfaindjhompbnflcldabbghjo?hl=en)
- [GateOne](https://github.com/liftoff/GateOne) [![stars](https://img.shields.io/github/stars/liftoff/GateOne.svg?style=social&label=stars)](https://github.com/liftoff/GateOne) - HTML5-powered terminal emulator and _SSH_ client.
- [KeyBox](https://github.com/skavanagh/KeyBox) [![stars](https://img.shields.io/github/stars/skavanagh/KeyBox.svg?style=social&label=stars)](https://github.com/skavanagh/KeyBox) - Web-based _SSH_ console that centrally manages administrative access to systems.
- [Apache Guacamole](https://guacamole.incubator.apache.org/) - Apache Guacamole is a HTML5 based clientless remote desktop gateway. It supports standard protocols like VNC, RDP, and SSH.
- [SSHmon](https://github.com/hpello/sshmon) [![stars](https://img.shields.io/github/stars/hpello/sshmon.svg?style=social&label=stars)](https://github.com/hpello/sshmon) - Real-time GUI to monitor SSH connections and establish port forwardings.

### Testing / Honeypots

- [ssh-hammer](https://github.com/shazow/ssh-hammer) [![stars](https://img.shields.io/github/stars/shazow/ssh-hammer.svg?style=social&label=stars)](https://github.com/shazow/ssh-hammer) - _SSH_ load testing tool.
- [kippo](https://github.com/desaster/kippo) [![stars](https://img.shields.io/github/stars/desaster/kippo.svg?style=social&label=stars)](https://github.com/desaster/kippo) - _SSH_ Honeypot.
- [cowrie](https://github.com/micheloosterhof/cowrie) [![stars](https://img.shields.io/github/stars/micheloosterhof/cowrie.svg?style=social&label=stars)](https://github.com/micheloosterhof/cowrie) - _SSH_ Honeypot (based on kippo).
- [sshmitm](http://linux.die.net/man/8/sshmitm) - _SSH_ monkey-in-the-middle.
- [ssh-audit](https://github.com/arthepsy/ssh-audit) [![stars](https://img.shields.io/github/stars/arthepsy/ssh-audit.svg?style=social&label=stars)](https://github.com/arthepsy/ssh-audit) - A tool for _SSH_ server auditing.
- [sshesame](https://github.com/jaksi/sshesame) [![stars](https://img.shields.io/github/stars/jaksi/sshesame.svg?style=social&label=stars)](https://github.com/jaksi/sshesame) - A fake SSH server that lets everyone in and logs their activity.

### Alternatives to _SSH_

- [GoTTY](https://github.com/yudai/gotty) [![stars](https://img.shields.io/github/stars/yudai/gotty.svg?style=social&label=stars)](https://github.com/yudai/gotty) - Share your terminal as web application.
- [telnet](http://www.telnet.org/htm/faq.htm) - An unencrypted network protocol and an application used to connect to remote computers and issue commands.
- [ttyd](https://github.com/tsl0922/ttyd) [![stars](https://img.shields.io/github/stars/tsl0922/ttyd.svg?style=social&label=stars)](https://github.com/tsl0922/ttyd) - Share your terminal over the web.
- [rsh](https://en.wikipedia.org/wiki/Remote_Shell) - An unencrypted network protocol and application used to connect to remote computers and issue commands.

## Libraries

- C/C++
  - [libssh](https://www.libssh.org) - The _SSH_ library.
- Golang
  - [crypto/ssh](https://godoc.org/golang.org/x/crypto/ssh) - Built-in _SSH_ client and server library.
  - [sftp](https://github.com/pkg/sftp) [![stars](https://img.shields.io/github/stars/pkg/sftp.svg?style=social&label=stars)](https://github.com/pkg/sftp) - _SFTP_ support for the go.crypto/ssh package.
  - [go-sshkit](https://github.com/shazow/go-sshkit) [![stars](https://img.shields.io/github/stars/shazow/go-sshkit.svg?style=social&label=stars)](https://github.com/shazow/go-sshkit) - Toolkit for building _SSH_ servers and clients in Go.
  - [Socker](https://github.com/cosiner/socker) [![stars](https://img.shields.io/github/stars/cosiner/socker.svg?style=social&label=stars)](https://github.com/cosiner/socker) - Library for Go to simplify the use of _SSH_.
  - [go-sshkeys](https://github.com/moul/go-sshkeys) - Golang SSH Keys manipulation library
- Java
  - [jsch](http://www.jcraft.com/jsch/) - Pure _java_, _BSD_ licensed, _SSH2_ client library.
- Javascript/Node.js
  - [ssh2](https://github.com/mscdex/ssh2) [![stars](https://img.shields.io/github/stars/mscdex/ssh2.svg?style=social&label=stars)](https://github.com/mscdex/ssh2) - _SSH2_ client and server modules written in pure _JavaScript_ for _node.js_.
- Python
  - [paramiko](https://github.com/paramiko/paramiko) [![stars](https://img.shields.io/github/stars/paramiko/paramiko.svg?style=social&label=stars)](https://github.com/paramiko/paramiko) - Native _Python_ _SSHv2_ protocol library.
- Ruby
  - [net-ssh](https://github.com/net-ssh/net-ssh) [![stars](https://img.shields.io/github/stars/net-ssh/net-ssh.svg?style=social&label=stars)](https://github.com/net-ssh/net-ssh) - Pure _Ruby_ implementation of an _SSH_ (protocol 2) client.

## Resources

### Tutorials

- [How to use _SSH_ to Connect to a Remote Server](https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-in-ubuntu)
- [Best practices](https://blog.0xbadc0de.be/archives/300)
- [Granting Temporary Access to Your Servers (Using Signed _SSH_ Keys)](http://linux-audit.com/granting-temporary-access-to-servers-using-signed-ssh-keys/)
- [How to SSH login without a password](https://www.rosehosting.com/blog/ssh-login-without-password-using-ssh-keys/)
- [Gist: SSH Recipes](https://gist.github.com/mjalajel/beaa91a5f8d04ebb464c2c28da01406a) - Collection of recipes for writing awesome ssh config files.

### Security

- [01/14/2016](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2016-0777) - Integer Overflow `CVE 2016 077[7-8]`.
- [Security/Guidelines/OpenSSH - MozillaWiki](https://wiki.mozilla.org/Security/Guidelines/OpenSSH) - `sshd\_config` for `6.7+`, `5.3`.
- [Applied-Crypto-Hardening](https://github.com/BetterCrypto/Applied-Crypto-Hardening) [![stars](https://img.shields.io/github/stars/BetterCrypto/Applied-Crypto-Hardening.svg?style=social&label=stars)](https://github.com/BetterCrypto/Applied-Crypto-Hardening) - `sshd\_config` for `6.X`

### Documentation

- [man page](http://linux.die.net/man/1/ssh)
- [Specifications (OpenSSH)](http://www.openssh.com/specs.html)
- [Wikipedia article](https://en.wikipedia.org/wiki/Secure_Shell)

### Community

- [StackOverflow](http://stackoverflow.com/questions/tagged/ssh)
- [ServerFault](http://serverfault.com/questions/tagged/ssh)

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Manfred Touron](https://github.com/moul) has waived all copyright and related or neighboring rights to this work.
