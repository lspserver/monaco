# monaco

[![Build Status](https://github.com/lspserver/monaco/workflows/CI/badge.svg?branch=main&event=push)](https://github.com/lspserver/monaco/actions?query=workflow%3ACI)
[![codecov](https://codecov.io/gh/lspserver/monaco/branch/main/graph/badge.svg?token=FS77A6KD37)](https://codecov.io/gh/lspserver/monaco)
[![License](https://img.shields.io/github/license/lspserver/monaco.svg?color=brightgreen)](https://github.com/lspserver/monaco/blob/main/LICENSE)
[![Tag](https://img.shields.io/github/tag/lspserver/monaco.svg?color=brightgreen)](https://github.com/lspserver/monaco/tags)
[![Gitter chat](https://badges.gitter.im/craftslab/lspserver.png)](https://gitter.im/craftslab/lspserver)



## Introduction

*monaco* is the client of [lspserver](https://github.com/lspserver) written in JavaScript.



## Run

```bash
# Set proxy
yarn config set proxy http://proxy_host:port
yarn config set https-proxy https://proxy_host:port

# Run client
git clone https://github.com/lspserver/monaco.git
cd monaco
export NODE_OPTIONS=--openssl-legacy-provider
yarn && yarn run start
```



## Docker

```bash
git clone https://github.com/lspserver/monaco.git

cd monaco
docker build --no-cache -f Dockerfile -t ghcr.io/lspserver/monaco:latest .
docker run --rm -p 4000:4000 ghcr.io/lspserver/monaco:latest
```



## License

Project License can be found [here](LICENSE).



## Reference

- [language-server-protocol](https://microsoft.github.io/language-server-protocol/)
- [monaco-editor](https://microsoft.github.io/monaco-editor/)
- [monaco-languageclient](https://github.com/TypeFox/monaco-languageclient)
- [vscode-json-languageservice](https://github.com/microsoft/vscode-json-languageservice)
