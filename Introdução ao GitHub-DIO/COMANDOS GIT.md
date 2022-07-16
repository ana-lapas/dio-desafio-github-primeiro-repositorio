# COMANDOS GIT

Windows utiliza comandos:

-cd

-dir

-mkdir

-del/rmdir

- Botão windows > cmd >Abre o terminal do windows na pasta padrão c:/user/nomedousuario;
- No windows tem um minicomando que entende linux;
- Dir (enter): Mostra a lista de diretórios (pastas);
- Todos os comandos possuem variancias (flags) que modificam o formato que os programas rodam;
- O comando cd nomedapasta / possibilita a navegação entre as pastas;
- cd.. retrocede um nível na navegação;
- O comando para limpar o terminal é o cls;
- Tab tem a função de completar;
- mkdir NomedaPasta é o comando para criar uma pasta;
- Comando: echo só retorna o que foi gigitado;
- Comando: echo hello > hello.txt (Cria o arquivo nomeado, caso ele não exista)
- Comando: del nomedoarquivo é utilizado para deletar o arquivo;
- Comando: rmdir nomedapasta /S /Q são duas flags para excluir;
- Comando: echo "olá mundo" | openssl sha1 fornece o stadin de 40 digitos (que gera a encriptação de um arquivo);
- Comando: openssl sha1 nomedoarquivo.ext gera o stadin de cada arquivo;

## OBJETOS INTERNOS

- BLOBS: echo -e ‘string’ | openssl1 sha1  (contém meta dado, tipo do objeto, tamanho do objeto (BLOB) \o e conteúdo) blob é um arquivo e qualquer alteração gera um sha1 diferente
- TREES (armazenam os blobs) contém metadado, aponta pra o blob (arquivos),  contém o nome do arquivo e o sha1, ou aponta para outra árvore
- COMMITS (pode apontar para tree, parente, autor, mensagem e o timesnap) tbm possui um sha1, qualquer alteração gera um sha1.

Esse sistema é distribuído e seguro, os commits são difíceis de serem alterados assim como as versões dos arquivos que estão nele. 

echo ‘string’ | git hash-object —stdin (gera o stdin da string)

## CHAVES SSH E TOKENS

Chave ssh é uma chave pública e uma privada (da nossa máquina que já fica configurada).