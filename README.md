Easily create Slackware chroot jail for testing and development SlackBuilds.
Its for Stable (32/64) bits and Current. Inspired by debootstrap.

## Why?
I use Slackware current, but as a SlackBuilds maintainer, i need to have Slackware stable installed to maintain the scripts in a clean environment.
Using Virtualization is a simple plan, but for compilation and testing it ends up making the environment "slower" even with KVM.
So this program does what I need, it creates a jailed environment, completely clean of 64-bit Slackware (Current or Stable).

## How use?

This tool is available on Slackbuilds
https://slackbuilds.org/repository/15.0/system/slackbootstrap/?search=slackboot

### Installation manually.

```
$ git clone https://github.com/slackjeff/slackbootstrap
$ cd slackbootstrap
# cp slackbootstrap /usr/local/sbin/
# mkdir /etc/slackbootstrap/

for 64 bits:
# cp slackbootstrap64.conf /etc/slackbootstap/slackbootstrap.conf

If your system is 32 bits:
# cp slackbootstrap32.conf /etc/slackbootstap/slackbootstrap.conf
```
