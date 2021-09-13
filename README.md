# packer-ansible-poc

This will create an aws spot instance and build a golden image based on what is provided in ansible

## Getting Started

1. Modify the variables at the top of `packer/demo.json` to reflect your infrastructure
1. From the Packer directory run `packer build -only=ec2-amazonlinux2 demo.json`. You can modify `-only` for other other supported operating systems.
1. Make sure, you have an AWS SSH Keypair for the instances. This module doesn't handle it.
