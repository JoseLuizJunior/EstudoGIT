# EstudoGIT

## Getting Started
**1 - Download git**

Windows: https://gitforwindows.org/

Linux: https://git-scm.com/download/linux

Mac: https://git-scm.com/download/mac

**2 - Configurações globais obrigatórias do git**

Usuario e email:
```
git config --global user.name  MEU NOME
git config --global user.email MEU_EMAIL@EMAIL.COM.BR
```

**3 - Criar um repositorio local**

Caso seja um repositorio novo.
```
git init
```

Caso for copiar, "clonar" um respositorio já existente:

```
git clone https://github.com/JoseLuizJunior/EstudoGIT.git
```

Ao clonar não seguir o passo 5.

**4- add e Commit.**

Marca todos os arquivo como tracked "rastreado" envia para stage area.
```
git add .
```

Marca um unico arquivo como tracked "rastreado".
```
git add nomeDoArquivo
```

Marca todos como tracked "rastreado", arquivo com extensão específica.
```
git add *.java
```

Envia arquivos tracked "rastreado" para o respositório local.
```
git commit -m "descrição do commit"
```

**5- Contectar repositorio local com repositorio remoto do github.**

```
git remote add origin https://github.com/JoseLuizJunior/EstudoGIT.git
```

Caso tenha algum arquivo commitado no repositorio remoto executar o seguinte comando:
```
git pull
```

Quando aparecer mensagem de merge apertar as teclas **ctrl + x**

**6 - Enviar arquivo para repositório remoto**

```
git push origin master
```

**7 - Visualizar histórico de commits**

Para navegar usar ENTER próxima linha, para sair usar tecla Q.

Exibe todo o histórico de commits realizados no repositório.
```
git log
```

Exibe histórico de commits simplificado.
```
git log --oneline
```

Exibe histórico e identifica os arquivos alterados.
```
git log --stat
```

**8 - Visualizar alterações de arquivos**

Exibe alterações feitas no arquivo ANTES de executar comando git add.
```
git diff nome_arquivo.txt
```

Exibe alterações feitas no arquivo DEPOIS de executar comando git add.
```
git diff --staged
```

**9 - Deletar arquivos commitados**

Remove arquivos que foram commitados; para concluir executar commit
```
git rm nome_arquivo.txt
```

**10 - Renomear/mover arquivos**

Renomea o arquivo sem gerar log de arquivo excluido
```
git mv nome_arquivo novo_nome_arquivo
```

Move o arquivo para o diretório pasta_nova
```
git mv nome_arquivo pasta_nova/nome_arquivo
```

**11 - Desfazer alterações**

Desfaz alterações de arquivos não rastreados
```
git checkout nome_arquivo.extensao
```

## Curiosidades

Comando commit -a ignora a etapa de rastrear o arquivo. Funciona somente para arquivos que já foram comitados.
```
git commit -am "descrição do commit"
```

Para não exibir arquivos não rastreados "untracked" configurar um arquivo chamado .gitignore
Link de Templates de .gitignore - https://github.com/github/gitignore
