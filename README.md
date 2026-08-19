# Laboratório de Administração de Sistemas Linux e Redes

Repositório dedicado à prática de comandos CLI, Shell Scripting, gerenciamento de permissões (FHS/Octal) e análise de logs.

## Conteúdo 1
- `backup.sh`: Script em Bash para rotina automatizada de backup comprimido do `etc`.
- `permissions_lab.sh`: Comandos e automação de permissões FHS e controle de acesso via grupos.

# Laboratório Prático: Linux & Git (Módulo 1)

Este documento contém os procedimentos práticos executados para fixação dos conceitos de estrutura FHS, comandos de navegação, permissões, gerenciamento de processos, logs, manipulação de arquivos e versionamento com Git.

---

## Parte 1: Revisando o Conteúdo Anterior

### 1.1. Gerenciamento de Processos e Sinais (`ps` e `kill -9`)
Criação de um processo em segundo plano, identificação do PID e encerramento forçado via sinal `SIGKILL`.

```bash
# 1. Cria um processo sleep por 500 segundos em background (&)
sleep 500 &

# 2. Localiza o PID do processo sleep
ps aux | grep sleep

# 3. Mata o processo usando o sinal SIGKILL (-9)
kill -9 <PID>

# 4. Confirma que o processo foi encerrado
ps aux | grep sleep
