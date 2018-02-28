# EstudoGIT

1 - Download git

Windows: https://gitforwindows.org/
Linux: https://git-scm.com/download/linux

2 - Configurações globais obrigatórias do git

Usuario e email:
git config --global user.name "MEU NOME"
git config --global user.email MEU_EMAIL@EMAIL.COM.BR

3 - Criar um repositorio local

git init

4- Contectar repositorio local com repositorio remoto do github.

git remote add origin https://github.com/JoseLuizJunior/EstudoGIT.git

Caso tenha algum arquivo commitado no repositorio remoto executar o seguinte comando:

git pull

quando aparecer mensagem de merge apertar as teclas ctrl + x

5 - Enviar arquivo para repositório remoto 

git push origin master

