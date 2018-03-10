# PSC

PSC is a CLI tool for publishing a local file as a Bitbucket Snippet.

## Usage

```
  psc [options] <file>

    Options:

      -h, --help                 output usage information
      -u, --username <username>  the user to authenticate as
      -p, --password <password>  the user's password
      -b, --browser              open the snippet in the system browser
```

## Installation

* Install [Node.js](https://nodejs.org/en "Node.js") and [npm](https://www.npmjs.com "npm")

* Run `npm install -g psc-tool`

* Run `psc --help` or `psc some_file` to upload it to Bitbucket.

## Credential management

The first time you upload a file you will be prompted for your Bitbucket username and password. These will be used to retrieve an OAuth refresh token which is stored in `~/.bitbucket-snippet` and used for subsequent requests. Treat this token carefully as it can be used to read and write snippets on your behalf.