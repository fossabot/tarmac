# TarMac
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdubo-dubon-duponey%2Ftarmac.svg?type=shield)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdubo-dubon-duponey%2Ftarmac?ref=badge_shield)


A very small wrapper to install & pre-configure Homebrew.

## TL;DR

```
bash -c "$(curl -fsSL https://raw.github.com/dubo-dubon-duponey/tarmac/master/init)"
```

Or get a local copy and `./init`.

You will be prompted for a github token, and optionally a "tmp" and "bin" path.

## Non-interactive

You can alternatively set the following environment variables:
 
 * `POSH_TOKEN`: github personal token to be used by brew
 * `POSH_TMP`: temporary directory to be used by brew, for eg `~/tmp`
 * `POSH_BIN`: final location of brew, for eg `~/Applications/bin`

Then call the script.

## After that...

Typically, migrating stuff from a template or another machine dump.

Dump it:
`brew bundle dump --file=MigrateBrewfile`

Load it:
`brew bundle install --file=MigrateBrewfile`

Or any other way to setup your environment.

## TODO

Test


## License
[![FOSSA Status](https://app.fossa.io/api/projects/git%2Bgithub.com%2Fdubo-dubon-duponey%2Ftarmac.svg?type=large)](https://app.fossa.io/projects/git%2Bgithub.com%2Fdubo-dubon-duponey%2Ftarmac?ref=badge_large)