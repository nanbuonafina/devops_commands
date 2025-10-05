# 🐧 Guia de 50 Comandos Linux para Devs

Este repositório contém uma lista prática com **50 comandos essenciais do Linux**, voltados especialmente para **desenvolvedores**, **estudantes de tecnologia** e **profissionais de DevOps**.

Organizados por categoria, eles ajudam a dominar o terminal e automatizar tarefas no ambiente Linux.

---

## 📁 1. Gerenciamento de Arquivos e Diretórios

| Comando | Descrição | Exemplo |
|----------|------------|---------|
| `ls` | Lista arquivos e diretórios | `ls -la` |
| `cd` | Muda de diretório | `cd /home/user` |
| `pwd` | Mostra o caminho atual | `pwd` |
| `mkdir` | Cria diretórios | `mkdir projetos` |
| `rmdir` | Remove diretórios vazios | `rmdir logs` |
| `cp` | Copia arquivos ou diretórios | `cp arquivo.txt backup/` |
| `mv` | Move ou renomeia arquivos | `mv index.html /var/www/` |
| `rm` | Remove arquivos ou diretórios | `rm -rf temp/` |
| `touch` | Cria arquivos vazios | `touch app.log` |
| `cat` | Exibe conteúdo de arquivos | `cat README.md` |
| `less` | Visualiza arquivos grandes paginados | `less /var/log/syslog` |
| `head` | Mostra as primeiras linhas de um arquivo | `head -n 10 arquivo.txt` |
| `tail` | Mostra as últimas linhas de um arquivo | `tail -f logs.txt` |
| `find` | Busca arquivos em diretórios | `find . -name "*.py"` |
| `grep` | Busca padrões dentro de arquivos | `grep "error" app.log` |

---

## 🔐 2. Permissões e Usuários

| Comando | Descrição | Exemplo |
|----------|------------|---------|
| `chmod` | Altera permissões de arquivos | `chmod 755 script.sh` |
| `chown` | Muda o dono e grupo de arquivos | `chown user:dev arquivo.txt` |
| `whoami` | Mostra o usuário atual | `whoami` |
| `sudo` | Executa comandos como superusuário | `sudo apt update` |
| `passwd` | Altera senha do usuário | `passwd` |

---

## ⚙️ 3. Informações do Sistema

| Comando | Descrição | Exemplo |
|----------|------------|---------|
| `uname -a` | Mostra informações do sistema operacional | `uname -a` |
| `top` | Monitora processos em tempo real | `top` |
| `htop` | Versão interativa do `top` | `htop` |
| `df -h` | Mostra uso do disco | `df -h` |
| `du -sh` | Mostra tamanho de um diretório | `du -sh /home/user` |
| `free -h` | Mostra uso da memória RAM | `free -h` |
| `uptime` | Tempo de atividade do sistema | `uptime` |
| `ps aux` | Lista processos em execução | `ps aux | grep python` |
| `kill` | Finaliza processos | `kill 1234` |
| `history` | Mostra histórico de comandos | `history` |

---

## 🌐 4. Rede

| Comando | Descrição | Exemplo |
|----------|------------|---------|
| `ping` | Testa conectividade com um host | `ping google.com` |
| `curl` | Faz requisições HTTP | `curl https://api.github.com` |
| `wget` | Baixa arquivos da web | `wget https://site.com/arquivo.zip` |
| `ifconfig` | Mostra interfaces de rede (antigo) | `ifconfig` |
| `ip addr` | Mostra IPs e interfaces | `ip addr show` |
| `netstat -tuln` | Mostra portas em uso | `netstat -tuln` |
| `ss -tuln` | Alternativa moderna ao netstat | `ss -tuln` |
| `scp` | Copia arquivos via SSH | `scp arquivo.txt user@host:/home/user` |
| `ssh` | Conecta a outro servidor Linux | `ssh user@192.168.0.10` |
| `traceroute` | Rastreia o caminho até um host | `traceroute google.com` |

---

## 🧩 5. Desenvolvimento e Automação

| Comando | Descrição | Exemplo |
|----------|------------|---------|
| `git` | Controle de versão | `git clone https://github.com/user/repo.git` |
| `make` | Executa tarefas automatizadas | `make build` |
| `docker` | Gerencia containers | `docker ps -a` |
| `npm` | Gerencia pacotes Node.js | `npm install express` |
| `pip` | Gerencia pacotes Python | `pip install flask` |
| `gcc` | Compila código C/C++ | `gcc main.c -o main` |
| `java` | Executa programas Java | `java Main` |
| `python3` | Executa scripts Python | `python3 script.py` |
| `bash` | Executa scripts Shell | `bash deploy.sh` |
| `cron` | Agenda tarefas automáticas | `crontab -e` |

---

## 📘 Dica Final

💡 **Combine comandos com pipes (`|`) e redirecionamentos (`>`, `>>`) para automatizar tarefas!**  
Exemplo:
```bash
grep "error" app.log | tail -n 5 > erros_recentes.txt
