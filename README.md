hackCO
======

## Getting Started

#### Clone & Init Gitmodules

First clone the repo:

```
git clone git@github.com:cScarlson/hackCO hackCO
cd !$
```

We're using a gitmodule for NDN.js - so you'll need to init this with:

```bash
git submodule init
git submodule update
```

Then, when there are upstream changes to the NDN module, you'll need to update again:

```bash
git submodule update
```

#### Install CCNx

You'll need to install CCNx.  Here's the official [docs](http://www.ccnx.org/documentation/).

If you're on OSX, this should be simple with `brew`.

```bash
brew install https://raw.github.com/dcunited001/homebrew/dc/ccn-keggar/Library/Formula/ccnx.rb
```

If you're on Linux, check out the official [install guide](https://www.ccnx.org/wiki/CCNx/InstallingCCNx).

> Basically, check out the list of dependencies and make sure you have them all.
> Use your package manager to download the ones you need, then download the CCNx source tarball.
> Then build from source and make sure the binaries end up in your path.
G
#### Install Node/NPM

On OSX:

```bash
brew install node
```

Verify with:

```bash
node --version
npm --version
```

#### Install Node/NPM

Using NPM:

```bash
npm install -g foreman
```

Now copy `Procfile.example` & `.env.example`

```bash
cp Profile.example Procfile
cp .env.example .env
```

#### Run CCNx & Node Server

Using Foreman:

```bash
nf start
```

#### View in [Browser](http://localhost:3000)

## Contributing

There's a few more dependencies you'll need to install to contribute.

#### Less

Less is a node module used to compile CSS assets.

To install:
```bash
npm install -g less
```
