# Importação das configurações do Neovim

## Criação da pasta de configurações

1. Navegar para a pasta HOME

   ```
   @yourusername:/$ cd ~/
   ```

2. Verificar se a pasta já contém o diretório de configurações

   ```
   @yourusernam:~$ ls
   ```

3. Caso não contenha, criar o diretório de configurações

   ```
   @yourusername:~$ mkdir .config
   ```

4. Acessar o diretório de configurações

   ```
   @yourusername:~$ cd .config
   ```

5. Verificar se existe o diretório de configurações do Neovim

   ```
   @yourusername:~/.config$ ls
   ```

6. Caso não exista, criar o diretório de configurações do Neovim

   ```
   @yourusername:~/.config$ mkdir nvim
   ```

7. Acessar o diretório de configurações do neovim

   ```
   @yourusername:~/.config$ cd nvim
   ```

8. Instalação do Github CLI client

   ```
   @yourusername:~/.config/nvim$ sudo dnf install gh
   ```

9. Após a instalação, realizar autenticação no github CLI

   ```
   @yourusername:~/.config/nvim$ gh auth login
   ? What account do you want to log into? GitHub.com
   ? What is your preferred protocol for Git operations on this host? HTTPS
   ? Authenticate Git with your GitHub credentials? Yes
   ? How would you like to authenticate GitHub CLI? Paste an authentication token
   Tip: you can generate a Personal Access Token here https://github.com/settings/tokens
   The minimum required scopes are 'repo', 'read:org', 'workflow'.
   ? Paste your authentication token: ************************************
   
   gh config set -h github.com git_protocol https
   ✓ Configured git protocol
   ✓ Logged in as douglasboardman
   ```

10. Salvamento das credenciais no cache

    ```
    @yourusername:~/.config/nvim$ git config --global credential.helper cache
    ```
