<h1>Comandos git</h1>

- Iniciar git
```
git init
```

- Configuração Local do Git
```
git config --<global ou local> user.name "<name user>"
git config --<global ou local> user.name <email@example.com>
```

- Adicionando um repositorio remoto (Obs: origin significa que é um repositório remoto e não local)
```
git remote add origin <URL>
```

- Baixar Commits, arquivos e refs de um repositório remoto para local
```
git fetch
```

- Ir para a branch master (a remota)
```
git checkout -f origin/master
```
ou
```
git checkout master
```
--------------------------------------------------------------------------------------
- Para restaurar um commit
```
git log --oneline
```
```
git restore --source <hash> <arquivo ou ponto para pegar todos>
```

- Para criar uma nova branch
```
git checkout -b <nome-branch>
```

- Ir (ou navegar) até uma branch
```
git switch <nome-branch>
```

- Após a primeira alteração commitada na branch local, pra enviar a branch com a alteração:
```
git push origin <nome-branch>
```

- Pra fazer merge<br>
-- Entra na branch que quer enviar 
```
git switch <nome-branch>
```
-- Realiza o merge da branch
```
git merge <nome-branch-que-quer-pegar>
```
