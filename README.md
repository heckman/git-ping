# git-ping

Test if git repository is available at a given URL.

## Usage

```text
usage: git ping URL

Returns a zero exit code if a git repository is found at the URL.
Produces no output.

Returns with a non-zero exit code if the repository is
not found or if the URL responds with a prompt for credentials.
Prompts will be suppressed. (Produces no output.)

If the URL does not begin with a URL scheme,
then a default base URL will be prepended,
and if it doesn't contain a "/" a default username
will also be added as a path segment after the base URL.

The defaults can be set with the environment variables
GIT_HOST and GIT_USER. If they are not set, default defaults are used.

Example: `GIT_HOST=https://github.com GIT_USER=heckman git ping git-ping`
will ping the URL 'https://github.com/heckman/git-ping'
```

## Installation

This script is in the bin directory. Put it on your system,
on the path is good—but it can be run from anywhere.

Set the `GIT_HOST` and `GIT_USER` environment variables to change the defaults,
or just edit the script.

## License

Shared under the MIT license.

It works on my machine. Use at your own risk.

If you do find any problems, please open an issue
or email me directly—my address is in the source.
