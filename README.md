# Laboratório: Instalar Software numa Distribuição Linux

> Laboratório do curso **"Tools of the Trade: Linux and SQL"** do **Google Cybersecurity Certificate** (Coursera / Qwiklabs).

## Objetivo

Usar o package manager **apt** com **sudo** para instalar, desinstalar e reinstalar aplicações de segurança de rede numa shell Bash, e confirmar que ficaram bem instaladas.

## Contexto

O laboratório corre numa máquina virtual com uma distribuição Linux baseada em Debian. Cenário: como analista de segurança, é preciso ter as ferramentas **nload** e **tcpdump** instaladas no sistema.

| Ferramenta | Para que serve |
| --- | --- |
| **nload** | Mostra o tráfego de rede em tempo real (entrada / saída) no terminal |
| **tcpdump** | Captura e analisa pacotes de rede pela linha de comandos, como o Wireshark mas sem janelas |

## Tarefas e comandos

### 1. Confirmar que o apt está instalado

```bash
apt
```

Se aparecer a versão e a lista de comandos, o apt está disponível.

### 2. Instalar o nload

```bash
sudo apt install nload
```

Confirmar com **Y** quando perguntar *"Do you want to continue?"*. Depois, escrever `nload` para o abrir (mostra Incoming / Outgoing) e sair com a tecla **q**.

### 3. Instalar o tcpdump

```bash
sudo apt install tcpdump
```

### 4. Listar as aplicações instaladas

```bash
apt list --installed
```

Procurar o **tcpdump** na lista para confirmar.

### 5. Desinstalar o nload

```bash
sudo apt remove nload
```

### 6. Reinstalar o nload

```bash
sudo apt install nload
```

## Resumo dos comandos

| Comando | O que faz |
| --- | --- |
| `apt` | Confirma que o apt existe |
| `sudo apt install <programa>` | Instala um programa |
| `sudo apt remove <programa>` | Desinstala um programa |
| `apt list --installed` | Lista o que está instalado |

## Conceitos aprendidos

- Uso do **apt** com **sudo** para instalar, remover e reinstalar software
- Confirmação de instalações com `apt list --installed`
- Para que servem o **nload** e o **tcpdump** no trabalho de um analista de segurança
- Uso de uma **máquina virtual** para praticar sem risco para o sistema real

## Resultado

✅ Laboratório concluído com sucesso, com todas as tarefas validadas no Qwiklabs.
