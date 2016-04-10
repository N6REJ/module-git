This a sub-repo of [Neard project](https://github.com/crazy-max/neard) involving Git tool bundles.

## Installation

* Download and install [Neard](https://github.com/crazy-max/neard).
* If you already have installed Neard, stop it.
* Download [a Git bundle](#download).
* Use a file archiver that supports [7z format](http://www.7-zip.org/7z.html) like [7zip](http://www.7-zip.org/) and extract the archive in `neard\tools\git\`.

Directory structure example :
```
[-] neard
 | [-] tools
 |  | [-] git 
 |  |  | [-] git1.8.4
 |  |     | neard.conf
```

* Edit the `neard.conf` file and replace the key `gitVersion` with the correct version.
* Start Neard.

## Download

![](https://raw.github.com/crazy-max/neard-tool-git/master/img/star-20160403.png) : Default bundle on Neard.

|               | Git release date | Neard release | Download |
| --------------|:----------------:|:-------------:|:--------:|
| **Git 1.8.4** ![](https://raw.github.com/crazy-max/neard-tool-git/master/img/star-20160403.png) | 2013/09/16 | [r1](https://github.com/crazy-max/neard-tool-git/releases/tag/r1) | [neard-git-1.8.4-r1.zip](https://github.com/crazy-max/neard-tool-git/releases/download/r1/neard-git-1.8.4-r1.zip) |

## Sources

* https://github.com/git-for-windows/git
* https://github.com/msysgit/msysgit

## Contribute

If you want to contribute to this bundle and create new bundles, you have to download [neard-dev](https://github.com/crazy-max/neard-dev) in the parent folder of the bundle.
Directory structure example :

```
[-] neard-dev
 | [-] build
 |  |  | build-commons.xml 
[-] neard-tool-git
 |  | build.xml
```

To create a new bundle :
* Do not forget to increment the `build.release` in the `build.properties` file.
* If you want you can change the `build.path` (default `C:\neard-build`).
* Open a command prompt in your bundle folder and call the Ant target `release` : `ant release`.
* Upload your release on a file hosting system like [Sendspace](https://www.sendspace.com/).
* Create an [issue on the Neard repository](https://github.com/crazy-max/neard/issues).

## Issues

Issues must be reported on [Neard repository](https://github.com/crazy-max/neard/issues).<br />
Please read [Found a bug?](https://github.com/crazy-max/neard#found-a-bug) section before reporting an issue.
