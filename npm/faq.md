1. npm install eAn unknown git error occurred
```text
npm ERR! npm ERR! code 128
npm ERR! npm ERR! An unknown git error occurred
npm ERR! npm ERR! command git --no-replace-objects ls-remote ssh://git@github.com/adobe-webplatform/eve.git
npm ERR! npm ERR! git@github.com: Permission denied (publickey).
npm ERR! npm ERR! fatal: Could not read from remote repository.

把自己的公钥配置到 github ssh 中即可
```