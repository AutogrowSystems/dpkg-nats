# NATS Debian Package builder

This repo uses ian to build a NATS package for Debian from the NATS Github releases page.

## Building

It can build for multiple architectures (currently amd64, arm64, armhf and armel) from the same repo:

    ian set -a amd64
    ian pkg -b
    
Then you will find a package in pkg/nats_1.0.4_amd64.deb.

    ian set -a armhf
    ian pkg -b
    
Then you will find a package in pkg/nats_1.0.4_armhf.deb.

    ian set -a arm64
    ian pkg -b
    
Then you will find a package in pkg/nats_1.0.4_arm64.deb.

    ian set -a armel
    ian pkg -b
    
Then you will find a package in pkg/nats_1.0.4_armel.deb.
