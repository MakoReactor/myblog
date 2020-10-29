---
title: "Wget Dicas De Uso"
date: 2020-10-28T15:44:04-03:00
draft: true
tags:
 - shell
 - bash
 - linux
categories:
 - Dicas Linux
---

### Instalar wget (Debian, Ubuntu, Linuxmint).

Caso a sua distro não venha com o comando wget instalado procure na documentação ou em fóruns a maneira correta de instalar o wget na sua distro. Cada distro tem uma forma ou comando diferente para instalar pacotes, a forma abaixo se aplica para distros baseadas em Debian e Ubuntu.

```bash
$> sudo apt install wget
```
Baixar uma página ou arquivo da internet.

Página
```bash
$> wget <url da página>
```

Arquivo
```bash
$> wget <url da página>.<arquivo>
```

Download vários arquivos salvos em um arquivo texto, cujo seja um arquivo como final do link.
```bash
$> wget -i arquivo_com_links_para_baixar.txt
```
Mudar o nome do arquivo no downlod.
```bash
$> wget -O nome_do_aquivo <url>
```

Baixando uma pasta online (ftp por exemplo).
```bash
$> wget -r ftp://servidor-ftp.com/diretório
```
Baixar site completo usando o wget

```bash
$> wget -m --convert-links --page-requisites <url-do-site>
```

