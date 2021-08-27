# Gitflow
[gitflow] https://github.com/nvie/gitflow

## O que é?
Uma forma de conseguir trabalhar com o Git de modo mais metodológico (branches)

## O que vai resolver
- Branch master apenas para produção
- Branch develop auxiliar da master - default
- Branch feature para issues (source develop e target master)
- Branch Release antes de colocar uma feature na master criar esta barnch e gerar uma tag (segura quais funcionalidades devem ir para produção)
- Branch Hotfix serve para correções de bug em produção (source master e target master e develop)

## Mão na massa
### Inicializar o repositório 
```bash
git flow init
```

### Criar uma feature
```bash
git flow feature start feature_name
```

### Finalizar uma feature
```bash
git flow feature finish feature_name
```
