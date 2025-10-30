# 🐧 Guia Prático de Comandos Linux

Este documento reúne os **principais comandos do Linux**, organizados por categoria, com exemplos e explicações.  
Ideal para iniciantes e desenvolvedores que desejam dominar o terminal.

---

## 🧭 Navegação e Informações do Sistema

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `pwd` | Mostra o caminho completo do diretório atual | `pwd` |
| `ls` | Lista arquivos e pastas | `ls -la` |
| `cd` | Navega entre diretórios | `cd /home/anderson` |
| `clear` | Limpa o terminal | `clear` |
| `whoami` | Exibe o usuário atual | `whoami` |
| `uname -a` | Mostra informações do sistema | `uname -a` |
| `history` | Exibe histórico de comandos | `history` |

---

## 📁 Manipulação de Diretórios e Arquivos

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `mkdir` | Cria um novo diretório | `mkdir projetos` |
| `rmdir` | Remove diretório vazio | `rmdir antigo` |
| `touch` | Cria um novo arquivo vazio | `touch index.html` |
| `cp` | Copia arquivos ou diretórios | `cp arquivo.txt backup/` |
| `mv` | Move ou renomeia arquivos | `mv arquivo.txt novo_nome.txt` |
| `rm` | Remove arquivos ou diretórios | `rm -rf pasta/` |
| `cat` | Exibe conteúdo de arquivos | `cat readme.md` |
| `less` | Mostra conteúdo paginado | `less log.txt` |
| `head` | Mostra primeiras linhas de um arquivo | `head -n 10 log.txt` |
| `tail` | Mostra últimas linhas de um arquivo | `tail -f log.txt` |

---

## 🔍 Busca e Filtros

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `find` | Localiza arquivos e diretórios | `find /home -name "*.txt"` |
| `grep` | Busca texto dentro de arquivos | `grep "erro" log.txt` |
| `locate` | Busca rápida por nome de arquivo | `locate arquivo.conf` |
| `wc` | Conta linhas, palavras e caracteres | `wc -l arquivo.txt` |
| `sort` | Ordena o conteúdo de arquivos | `sort lista.txt` |
| `uniq` | Remove linhas duplicadas | `uniq nomes.txt` |
| `diff` | Compara arquivos | `diff arquivo1.txt arquivo2.txt` |

---

## 🔐 Permissões e Usuários

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `chmod` | Altera permissões | `chmod 755 script.sh` |
| `chown` | Altera dono do arquivo | `chown anderson arquivo.txt` |
| `su` | Troca de usuário | `su root` |
| `sudo` | Executa comandos como superusuário | `sudo apt update` |
| `adduser` | Cria novo usuário | `sudo adduser maria` |
| `passwd` | Altera senha de usuário | `passwd maria` |

---

## ⚙️ Processos e Gerenciamento

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `ps` | Lista processos ativos | `ps aux` |
| `top` | Mostra processos em tempo real | `top` |
| `htop` | Versão avançada do top (instalar antes) | `htop` |
| `kill` | Encerra processo por PID | `kill 1234` |
| `pkill` | Encerra processos por nome | `pkill firefox` |
| `bg` / `fg` | Move processo para segundo ou primeiro plano | `fg` |
| `jobs` | Mostra processos em background | `jobs` |

---

## 🌐 Rede e Conexões

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `ping` | Testa conectividade com host | `ping google.com` |
| `ifconfig` | Mostra interfaces de rede (ou `ip a`) | `ifconfig` |
| `curl` | Faz requisições HTTP | `curl https://api.github.com` |
| `wget` | Baixa arquivos da internet | `wget https://arquivo.zip` |
| `netstat` | Mostra conexões e portas (deprecated: use `ss`) | `netstat -tuln` |
| `ss` | Exibe conexões de rede | `ss -tuln` |
| `scp` | Copia arquivos via SSH | `scp arquivo.txt user@192.168.1.1:/home/user/` |
| `ssh` | Acessa servidor remoto | `ssh user@192.168.1.1` |

---

## 📦 Gerenciamento de Pacotes

### **Debian / Ubuntu (APT)**
| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `sudo apt update` | Atualiza lista de pacotes | `sudo apt update` |
| `sudo apt upgrade` | Atualiza pacotes instalados | `sudo apt upgrade` |
| `sudo apt install` | Instala pacote | `sudo apt install git` |
| `sudo apt remove` | Remove pacote | `sudo apt remove nginx` |
| `sudo apt autoremove` | Remove dependências não usadas | `sudo apt autoremove` |

### **Fedora / CentOS (YUM / DNF)**
| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `sudo dnf install` | Instala pacote | `sudo dnf install vim` |
| `sudo dnf remove` | Remove pacote | `sudo dnf remove httpd` |

---

## 💾 Sistema de Arquivos e Disco

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `df -h` | Mostra uso de disco | `df -h` |
| `du -sh` | Mostra tamanho de diretório | `du -sh /var/log` |
| `mount` | Monta dispositivos | `mount /dev/sdb1 /mnt/usb` |
| `umount` | Desmonta dispositivos | `umount /mnt/usb` |
| `lsblk` | Lista discos e partições | `lsblk` |
| `fdisk -l` | Exibe detalhes das partições | `sudo fdisk -l` |

---

## 🧰 Outros Comandos Úteis

| Comando | Descrição | Exemplo |
|----------|------------|----------|
| `echo` | Exibe mensagens ou grava texto | `echo "Olá, Linux!"` |
| `date` | Mostra data e hora | `date` |
| `cal` | Exibe calendário | `cal 2025` |
| `alias` | Cria atalhos de comandos | `alias ll='ls -la'` |
| `reboot` | Reinicia o sistema | `sudo reboot` |
| `shutdown` | Desliga o sistema | `sudo shutdown now` |

---

## 🧩 Dicas Extras

- Use **`man comando`** para ver o manual completo de um comando.  
  👉 Exemplo: `man ls`
- Combine comandos com **pipes (`|`)**:  
  👉 Exemplo: `ps aux | grep nginx`
- Redirecione saída para arquivo:  
  👉 `ls > lista.txt`

---

## 📚 Referências

- [GNU Manual](https://www.gnu.org/manual/)
- [Linux Command Library](https://linuxcommandlibrary.com/)
- [Cheat.sh - Linux Cheatsheet](https://cheat.sh/)

---

**Autor:** Anderson Gouveia Lignelli  
**Licença:** MIT  


## Linux Estudos

echo "hello World" = Saída "hello World"

whoami - Para Verificar o usuario

id - Informações do usuario

uid - Seu ID de usuário(um indentificador numérico exclusivo)

gid: Seu ID de grupo principal

groups: Todos os grupos dos quais vocÊ é membro

root - é o superusuario -cpmo o administrador do sistema

apt - é um gerenciador de pacote

sudo apt update - instalação garante a versão mais recente do htop

sudo apt install - instalação a lista de pacotes
 
sudo apt install htop - instalação do htop htop

htop - informações sobre a a atividade do computador

q - para sair

pwd - "imprimir o diretóro de trabalho "abre o diretorio atual 

echo + ~ = abre o diretorio inical

ls - listará o os arquivos do diretórios

cd "nome da pasta" : Vou até ela

cd .. = rertorna para o diretorio anterior

touch file1.txt = Para criar um arquivo dentro da pasta

echo "Hello, Linux" > file2.txt = Cria o arquivo e coloca o texto dentro

echo "Hiden file"> .hiddenfile

mkdir testdir = Criando um novo diretório "Pasta"
 
ls -a = Monstra todo conteudo oculto

ls -la = Monstra = Monstra o formato longo com exibiçao de todos arquivos

ls -l = Mostra o conteudo criado com mkdir tesdir

cd /home/labex/project - Lembrar



 







