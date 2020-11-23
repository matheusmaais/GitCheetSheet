Configurando o git

Definindo nome de usuario e email
```
git config —-global user.name “meu nome”
git config —-global user.email “meu email”
```

Conferindo as configurações:
```
git config user.name
git config user.email
git config —-list
```

Qual editor to usando?
```
git config —-global core.editor “meu editor ” ex: vscode.. vim.. nano
```

---

Verificar o que foi modificado ou se tem arquivos não tracked
```
git status
```
Inicializar git em um diretório
```
git add .
Ou
git add -A ( adiciona TUDO )
```

Comitar uma alteração
```
git commit -m “descrição da alteração”
```

Comitar sem precisar digitar o add . Ou add -A
```
git commit -am “descriçao"
```

Revertendo commits ( voltar ao código que era antes do seu commit)
Desfazendo as cagadas!!
```
git log ( vai aparecer os commits anteriores, verificar qual é o seu commit bugado)
git reset --soft ( volta para o estado antes do commit anterior)
git reset --mixed ( mesma coisa do -soft só que precisa dar o comando add antes)
git reset --hard ( ignora tudo e qualquer coisa do ultimo commit, no caso voltaria pro penúltimo)  

Ex:
git reset  --hard ID_DO_COMMIT
```

---
BRANCHES

Listando as branches do repositório
```
git branch
```

Criando e entrando em uma nova branche
```
git checkout -b nome_da_branch
```

Trocando de branch
```
git checkout nome_da_branch
```

---
Diferenças entre os commits

Git status diz quais os arquivos foram alterados, mas não o que realmente foi alterado em cada arquivo.

```
git diff
```














