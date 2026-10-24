# GS/OS Consortium

Check out these two branches.

| Repository | Branch |
|---|---|
| [gsos](https://github.com/GS-OS-Consortium/gsos) | [`rel/6.0.4`](https://github.com/GS-OS-Consortium/gsos/tree/rel/6.0.4) |
| [iigs-programmers-workshop](https://github.com/GS-OS-Consortium/iigs-programmers-workshop) | [`linkiigs-1.3`](https://github.com/GS-OS-Consortium/iigs-programmers-workshop/tree/linkiigs-1.3) |

`gsos` is the System 6.0.4 rebuild. It is private and holds Apple's source and disks. `iigs-programmers-workshop` is the public Go toolchain; `linkiigs-1.3` is linkiigs 1.3.

`gsos` carries the toolchain as the `iigs-tools` submodule, cloned from this organization's repository. The commit recorded on `rel/6.0.4` is older than `linkiigs-1.3`, so check that branch out after cloning.

```sh
git clone -b rel/6.0.4 --recurse-submodules git@github.com:GS-OS-Consortium/gsos.git
cd gsos
git -C iigs-tools checkout linkiigs-1.3
```

For the toolchain alone:

```sh
git clone -b linkiigs-1.3 git@github.com:GS-OS-Consortium/iigs-programmers-workshop.git
```
