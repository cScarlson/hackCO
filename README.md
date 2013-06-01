hackCO
======


## Getting Started

#### Install CCNx

You'll need to install CCNx.  Here's the official [docs](http://www.ccnx.org/documentation/).

If you're on OSX, this should be simple with `brew`.

```bash
brew install https://raw.github.com/dcunited001/homebrew/dc/ccn-keggar/Library/Formula/ccnx.rb
```

If you're on Linux, check out the official [install guide](https://www.ccnx.org/wiki/CCNx/InstallingCCNx).

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
