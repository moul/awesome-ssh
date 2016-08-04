# Awesome SSH [![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)

> A curated list of SSH [apps](#apps), [libraries](#libraries) and [resources](#resources).

<h2 align="center"><img src="https://raw.githubusercontent.com/moul/awesome-ssh/master/logo.jpg" width="400" /></h2>

Inspired by the [awesome](https://github.com/sindresorhus/awesome) list thing.

Please read the [contribution guidelines](CONTRIBUTING.md) if you want to contribute.

**Check out my [blog](http://manfredtouron.tumblr.com) 🦄 or say *hi* on [Twitter](https://twitter.com/moul).**

## Table of Contents

- [Apps](#apps)
  - [`.ssh/config`](#sshconfig)
  - [Tools using the SSH protocol](#tools-using-the-ssh-protocol)
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

* [advanced-ssh-config](https://github.com/moul/advanced-ssh-config): a transparent wrapper (ProxyCommand) that adds regex, aliases, gateways, includes, dynamic hostnames to SSH and ssh-config.
* [storm](https://github.com/emre/storm): Manage your SSH like a boss.
* [ansible-ssh-config](https://github.com/gaqzi/ansible-ssh-config): Letting Ansible manage ssh config.
* [ec2ssh](https://github.com/mirakui/ec2ssh): A ssh_config manager for AWS EC2.
* [ssh-config](https://github.com/dbrady/ssh-config): A tool to help manage your .ssh/config file.

### Tools using the SSH protocol

* [ssh-chat](https://github.com/shazow/ssh-chat): Chat over SSH.
* [scp](http://linux.die.net/man/1/scp): secure remote file copy utility over SSH.
* [rsync](https://rsync.samba.org): fast incremental transfer utility that supports SSH.
* [sftp](https://en.wikipedia.org/wiki/SSH_File_Transfer_Protocol): file transfer protocol over SSH.
* [curl](http://curl.haxx.se): command line tool and library to transfer data (support sftp).

### Servers

* [ssh2docker](https://github.com/moul/ssh2docker): SSH server to Docker containers.
* [whosthere](https://github.com/FiloSottile/whosthere): A ssh server that knows who you are. `$ ssh whoami.filippo.io`.
* [sshfront](https://github.com/gliderlabs/sshfront): Programmable SSH frontend
* [ssh-chat](https://github.com/shazow/ssh-chat) - Chat over SSH.
* [sshcommand](https://github.com/dokku/sshcommand) - Turn SSH into a thin client specifically for your app
* [sshmuxd](https://github.com/joushou/sshmuxd) - sshmux frontend
* [x84](https://github.com/jquast/x84) - A python telnet/ssh server for modern UTF-8 and classic cp437 network virtual terminals. In spirit of classic software such as ami/x, teleguard, renegade, iniquity. http://x84.readthedocs.org/

### Network

* [Mosh](https://mosh.mit.edu) - The mobile shell.
* [sshfs](https://github.com/libfuse/sshfs): Filesystem client based on the SSH File Transfer Protocol.
* [ngrok](https://github.com/inconshreveable/ngrok): Introspected tunnels to localhost.
* [localtunnel](https://github.com/progrium/localtunnel): Expose localhost servers to the Internet.
* [sshuttle](https://github.com/apenwarr/sshuttle) - Transparent proxy server that works as a poor man's VPN. Forwards over ssh. Doesn't require admin. Works with Linux and MacOS. Supports DNS tunneling.
* [sshttp](https://github.com/stealth/sshttp) - SSH/HTTP(S) multiplexer. Run a webserver and a sshd on the same port w/o changes.
* [switcher](https://github.com/jamescun/switcher) - Run SSH and HTTP(S) on the same port
* [sslh](https://github.com/yrutschle/sslh) - Applicative Protocol Multiplexer (i.e: SSH + HTTPS)
* [tund](https://github.com/aphyr/tund) - SSH reverse tunnel daemon
* [autossh](http://www.harding.motd.ca/autossh/) - Automatically respawn ssh session after network interruption.
* [wssh](https://github.com/aluzzardi/wssh) - SSH to WebSockets Bridge
* [docker-volume-sshfs](https://github.com/vieux/docker-volume-sshfs) - sshfs docker volume plugin.

### Multiplexers

* [tmux](https://tmux.github.io): Terminal multiplexer.
* [clusterssh](https://github.com/duncs/clusterssh) - Cluster Admin Via SSH
* [tmux-cssh](https://github.com/dennishafemann/tmux-cssh): TMUX with a "ClusterSSH"-like behavior.
* [tm](https://github.com/Ganneff/tm): tmux manager / helper
* [i2cssh](https://github.com/wouterdebie/i2cssh) - csshX like ssh tool for iTerm2
* [ClusterSSH](http://sourceforge.net/projects/clusterssh/) - Controls a number of xterm windows via a single graphical console.

### SSH keys / Authentication

* [authy-ssh](https://github.com/authy/authy-ssh) - Easy two-factor authentication for ssh servers
* [github-auth](https://github.com/chrishunt/github-auth) - SSH key management for GitHub users.
* [cipherhub](https://github.com/substack/cipherhub) - Encrypt messages based on SSH public keys with easy import from GitHub
* [Slack notifications](http://www.ryanbrink.com/slack-ssh-session-notifications/) - Guide to setup Slack notifications (can be modified for other services).
* [totp-ssh-fluxer](https://github.com/benjojo/totp-ssh-fluxer) - A way to make sure your sshd port changes every 30 seconds

### SSH agent

* [ssh-ident](https://github.com/ccontavalli/ssh-ident) - Different agents and different keys for different projects, with ssh.
* [oh-my-zsh/plugins/ssh-agent](https://github.com/robbyrussell/oh-my-zsh/tree/master/plugins/ssh-agent) - ssh-agent plugin for ZSH.

### Tools

* [sshrc](https://github.com/Russell91/sshrc) - bring your .bashrc, .vimrc, etc. with you when you `ssh`

### Automation

* [ansible](https://github.com/ansible/ansible) - App deployment, configuration management and orchestration over SSH.
* [rtop](https://github.com/rapidloop/rtop) - Interactive, remote system monitoring tool based on SSH.
* [DSH - Dancer's shell / distributed shell](https://www.netfort.gr.jp/~dancer/software/dsh.html.en) - Wrapper for executing multiple remote shell commands from one command line.
* [parallel-ssh](https://code.google.com/p/parallel-ssh/) - Provides parallel versions of OpenSSH and related tools.
* [SSH Power Tool](https://code.google.com/p/sshpt/) - Execute commands and upload files to many servers simultaneously without using pre-shared keys.

### Web

* [Secure Shell chrome extension](https://chrome.google.com/webstore/detail/secure-shell/pnhechapfaindjhompbnflcldabbghjo?hl=en)
* [GateOne](https://github.com/liftoff/GateOne) - HTML5-powered terminal emulator and SSH client
* [KeyBox](https://github.com/skavanagh/KeyBox) - web-based SSH console that centrally manages administrative access to systems.

### Testing / Honeypots

* [ssh-hammer](https://github.com/shazow/ssh-hammer) - SSH load testing tool.
* [kippo](https://github.com/desaster/kippo) - SSH Honeypot
* [cowrie](https://github.com/micheloosterhof/cowrie) - SSH Honeypot (based on kippo)
* [sshmitm](http://linux.die.net/man/8/sshmitm) - SSH monkey-in-the-middle

### Alternatives to SSH

* [GoTTY](https://github.com/yudai/gotty): Share your terminal as web application
* [telnet](http://www.telnet.org/htm/faq.htm): An unencrypted network protocol and an application used to connect to remote computers and issue commands.
* [rsh](https://en.wikipedia.org/wiki/Remote_Shell): An unencrypted network protocol and application used to connect to remote computers and issue commands.

## Libraries

* C/C++
  * [libssh](https://www.libssh.org): The SSH library.
  * [substack/libssh](https://github.com/substack/libssh): multiplatform C library implementing the SSHv2 and SSHv1 protocol on client and server side.
* Golang
  * [crypto/ssh](https://godoc.org/golang.org/x/crypto/ssh) - built-in SSH client and server library.
  * [sftp](https://github.com/pkg/sftp) - SFTP support for the go.crypto/ssh package.
  * [go-sshkit](https://github.com/shazow/go-sshkit) - Toolkit for building SSH servers and clients in Go.
* Java
  * [jsch](http://www.jcraft.com/jsch/) - pure java, BSD licensed, SSH2 client library.
* Javascript/Node.js
  * [ssh2](https://github.com/mscdex/ssh2) - SSH2 client and server modules written in pure JavaScript for node.js
* Python
  * [paramiko](https://github.com/paramiko/paramiko): Native Python SSHv2 protocol library.
* Ruby
  * [net-ssh](https://github.com/net-ssh/net-ssh) - Pure Ruby implementation of an SSH (protocol 2) client

## Resources

### Tutorials

* [How to use SSH to Connect to a Remote Server](https://www.digitalocean.com/community/tutorials/how-to-use-ssh-to-connect-to-a-remote-server-in-ubuntu)
* [Best practices](https://blog.0xbadc0de.be/archives/300)
* [Granting Temporary Access to Your Servers (Using Signed SSH Keys)](http://linux-audit.com/granting-temporary-access-to-servers-using-signed-ssh-keys/)

### Security

* [01/14/2016](https://web.nvd.nist.gov/view/vuln/detail?vulnId=CVE-2016-0777) - Integer Overflow CVE 2016 077[7-8]
* [Security/Guidelines/OpenSSH - MozillaWiki](https://wiki.mozilla.org/Security/Guidelines/OpenSSH) - sshd\_config for 6.7+, 5.3
* [Applied-Crypto-Hardening](https://github.com/BetterCrypto/Applied-Crypto-Hardening/tree/master/src/configuration/SSH/OpenSSH) - sshd\_config for 6.X

### Documentation

* [man page](http://linux.die.net/man/1/ssh)
* [Specifications (OpenSSH)](http://www.openssh.com/specs.html)
* [Wikipedia article](https://en.wikipedia.org/wiki/Secure_Shell)

### Community

* [StackOverflow](http://stackoverflow.com/questions/tagged/ssh)
* [ServerFault](http://serverfault.com/questions/tagged/ssh)

## License

[![CC0](https://i.creativecommons.org/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, [Manfred Touron](https://github.com/moul) has waived all copyright and related or neighboring rights to this work.
