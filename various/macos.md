# MacOS

Various stuff about MacOS/Homebrew/whatever.

## Error : Xcode outdated and need a beta version

Happened while using MacOS Catalina and trying to install `php@7.3` using Homebrew

```console
$ Error: Your Xcode (10.3) is too outdated.
$ Please update to Xcode 11.0 (or delete it).
```

**Solution**

If the requested version of Xcode is not installed, install it in the Applications folder and change the default version of Xcode that's used and install the command-line tools related to this version.

Then, run 
```console
$ sudo xcode-select -s /Applications/Xcode-beta.app
$ xcode-select --install
```

After that, I was able to use Homebrew without problems.