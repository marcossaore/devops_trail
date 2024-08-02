# O que é Linux?

**Linux** é um sistema operacional de código aberto, baseado no kernel Linux, que é o núcleo do sistema. Foi criado por Linus Torvalds em 1991 e é mantido por uma comunidade de desenvolvedores ao redor do mundo. Linux é conhecido por sua estabilidade, segurança e flexibilidade, sendo amplamente utilizado em servidores, desktops, dispositivos móveis, e muito mais.

## Principais Características

1. **Código Aberto (Open Source):** O código-fonte do Linux é livremente disponível para qualquer pessoa. Isso permite que desenvolvedores personalizem e modifiquem o sistema conforme suas necessidades.

2. **Multiplataforma:** Linux pode ser executado em uma ampla variedade de hardwares, desde PCs e servidores até dispositivos móveis, sistemas embarcados e supercomputadores.

3. **Segurança:** Linux é conhecido por seu alto nível de segurança, com permissões de usuário rigorosas e uma comunidade ativa que rapidamente corrige vulnerabilidades.

4. **Estabilidade e Desempenho:** É frequentemente escolhido para ambientes de servidor e sistemas críticos devido à sua estabilidade e capacidade de gerenciamento eficiente de recursos.

5. **Distribuições (Distros):** Existem muitas distribuições Linux (ou "distros"), que são variações do sistema com diferentes conjuntos de softwares e funcionalidades. Exemplos incluem Ubuntu, Fedora, Debian, CentOS e Arch Linux.

## Usos Comuns

- **Servidores:** Linux é amplamente usado para hospedagem de sites, servidores de e-mail, bancos de dados, e aplicações empresariais.
- **Desktops e Laptops:** Muitas distribuições oferecem interfaces amigáveis para uso diário em desktops e laptops.
- **Desenvolvimento de Software:** É uma escolha popular para desenvolvedores devido ao seu rico conjunto de ferramentas de programação e suporte a diversas linguagens.
- **Sistemas Embarcados:** Utilizado em dispositivos como roteadores, smart TVs, sistemas de infotainment automotivos e muito mais.
- **Supercomputadores:** A maioria dos supercomputadores do mundo roda Linux devido à sua eficiência e capacidade de personalização.

## Vantagens de Usar Linux

- **Custo:** Linux é geralmente gratuito, o que reduz os custos de licenciamento de software.
- **Flexibilidade:** Pode ser personalizado para atender a necessidades específicas, tanto em termos de software quanto de hardware.
- **Comunidade e Suporte:** Uma grande comunidade de usuários e desenvolvedores proporciona suporte contínuo e contribuições para a melhoria do sistema.

Linux é uma plataforma poderosa e versátil que continua a crescer em popularidade, graças à sua confiabilidade, segurança e a liberdade que oferece aos usuários.

Para mais informações, visite o [site oficial do Linux](https://www.kernel.org/).

## Sumário

- [Gerenciador de pacotes](#gerenciador-de-pacotes)
- [Comandos](./commands/about.md)

# Gerenciador de pacotes

É um utilitário para gerenciar pacotes do sistema operacional, é usado para instalar e remover pacotes e para atualizar o sistema. Cada distro tem sua biblioteca de pacotes como por exemplo `apt-get` do Debian/Ubuntu (.deb) ou `yum` do CentOS (.rpm).

## Exemplo com Ubuntu

```bash	
sudo apt-get update # atualiza os pacotes no repositório da distro
sudo apt-get install apache2 # instala o pacote apache2
sudo apt-get remove apache2 # remove o pacote apache2
sudo apt-get upgrade # atualiza o sistema
sudo apt-cache show vim # mostra informações sobre o pacote
sudo apt-cache search nginx # procura pacotes
```

Use o DistroWatch para saber como instalar e remover pacotes de acordo com o sistema operacional.(
[DistroWatch Package Manager](https://distrowatch.com/dwres.php?resource=package-management))