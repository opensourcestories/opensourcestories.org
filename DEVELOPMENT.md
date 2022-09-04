# Development

This document describes how to get the opensourcestories.org site running locally.

## Getting started

This repository provides a devcontainer to make getting started with development easy. This supports running the development environment as a container locally with VSCode. This will spin up a hugo server and allow for local development with live code reloading without any dependencies on your local environment.

**NOTE**: You can specify the version of Hugo to use in the `devcontainer.json` file. However it is recommended to use v0.102.0 or above to support commonly used development environments (arm64,amd64, etc.).

### Using VSCode

To get started with VSCode, you'll first need to ensure that you have the `Remote Development` extension pack installed. From there, all you'll need to do is launch `code` from the root of this repository. Once launched, VSCode will notice the existence of the .devcontainer directory and ask you to reopen the current folder to develop in a container. At this point, VSCode will relaunch and build the container if necessary. Once the container is built, your hugo server will be launched and you'll be able to access the current site at `http://localhost:1313`.
