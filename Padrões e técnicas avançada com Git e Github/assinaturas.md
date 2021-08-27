# GPG

## Gerar chave
- Listar chaves
```bash
 gpg --list-secret-keys --keyid-format LONG
```

- nova chave
```bash
gpg --full-generate-key
```

- Visualizar a public key
```bash
gpg --armor --export DA179636FA27C823
```

- Garantir assinatura pelo git
```bash
git config --global user.signingKey DA179636FA27C823
``` 

- Activar ggp tty in $HOME/.bash_profile
```bash
export GPG_TTY=$(tty) 
```

- Definir assinatura por padrão global commint e tags
```bash
git config --global commit.gpgSign true
git config --global tag.gpgSign true
```