# Upcode CLI - BASH

## Como baixar e executar

```bash
# Cria alias para baixar e executar.
echo 'alias upcode="curl -s \"https://raw.githubusercontent.com/feerdinando/uploader-tool/refs/heads/main/upcode.sh?v=\$(date +%s)\" | bash"' >> ~/.bashrc

# Recarrega o bash
source ~/.bashrc

# Inicializa com o alias definido
upcode
```

Com esse comando, um alias é definido para facilitar a inicialização. Depois disso, basta chamar a palavra-chave definida no terminal para abrir o Upcode.

Ao iniciar, o Upcode verifica automaticamente algumas dependências, especialmente o **FZF**, responsável pela renderização dos menus. Caso o FZF não esteja instalado, utilize um gerenciador de pacotes para instalar facilmente:

```bash
choco install fzf
# ou
scoop install fzf
```

> **Observação:** O VSCode precisa estar com permissão de administrador para instalar, ou você pode realizar a instalação manualmente via terminal (também como administrador).

Se houver problemas com múltiplos aliases, acesse o arquivo principal do bash com um editor e remova o alias desejado. Exemplo:

```bash
code ~/.bashrc
```

A palavra no início representa o editor: `code` (VSCode), `notepad`, `nano`, etc.

Para recarregar o arquivo de configuração do bash, utilize:

```bash
source ~/.bashrc
```

Após a instalação, serão solicitadas credenciais de login, realizando uma requisição para o endpoint de autorização. Após o login, os menus ficarão disponíveis para uso normalmente.
