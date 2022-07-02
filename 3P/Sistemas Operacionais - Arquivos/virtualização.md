# Conceito
Virtualização é o conceito de implementar uma plataforma virtual via software que reproduz o comportamento de uma máquina na vida real.

# Técnicas de virtualização

## Virtual Machine Monitors (VMMs)
Oferecem um framework em software que é idêntico ao hardware real. Os VMMs não são parte do conceito de virtualização em nível de linguagem de programação (JVM, .NET).

### Virtualização Total
O VMM encontra-se instalado sobre um outro sistema operacional instalado (SO hospedeiro). Por exemplo:
- VMWare Player
- VirtualBox
- Parallels Desktop

### Para-virtualização
O VMM é representado por um módulo (hypervisor) que é instalado diretamente sobre o hardware. Por exemplo:
- VMWare vSphere Hypervisor
- Microsoft Hyper-V
- XEN
- KVM

Obs: Docker não é virtualização, ao contrário do que muitos pensam.

# Vantagens da virtualização
- Manutenção de sistemas legados desenvolvido com tecnologias antigas.
- Criação facilitada de ambientes (produção-homologação-testes).
- Facilidade de implementação de cópia de segurança (backup).
- Balanceamento de carga.
- Write once, run everywhere.
- Virtualização com suporte de hardware.
