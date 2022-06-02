
# Github Actions e Terraform com OCI
[![Github](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/lucianosilva/oci-terraform-sample1)

Objetivo deste repositório é mostrar o provisionamento de recursos no OCI (Oracle Cloud Infrastructure), utilizando o Github Actions como pipeline e Terraform.

- [Terraform](#o-que-é-terraform-)
- [Pré-requisitos](#pré-requisitos)
- [Obtendo credenciais](#obtendo-credenciais)
- [Contato](#contato)

## O que é Terraform? 🗒
Terraform é uma ferramenta de software livre de "infraestrutura como código" criada pela HashiCorp.
Permite aos desenvolvedores usar uma linguagem de configuração de alto nível (programação declarativa) chamada HCL para descrever a infraestrutura na cloud para executar um aplicativo.

Através dos provedores do Terraform, ou seja, plugins que implementam tipos de recursos capazes de comunicar com o ambiente cloud do provedor. Sendo assim, o Terraform é capaz de implementar em ambientes de cloud híbrida ou multicloud.

## Pré-requisitos

- [x] Criar uma conta no <a href="https://www.oracle.com/br/cloud/free/">Always Oracle Cloud Free</a>.
- [x] Se você estiver trabalhando no Windows, instale o `Git Bash`.
- [x] Instalar o `OCI CLI`.
- [x] Instalar o `Terraform`.

## Obtendo credenciais
Acesse sua conta no OCI (http://cloud.oracle.com), efetue o login e siga os passos abaixo. Você deverá obter as seguintes informações:
```
- Tenancy OCID
- Region
- Compartment OCID
- User OCID
- Username
- User Auth Token
```

- Canto superior direito clique no menu Profile, em seguida clique no Tenancy.
<p align="center"><img src="static/oci-screen1.png" alt="Profile Menu"></p>

- Na página de informação do Tenancy, clique em Copy e salve o `Tenancy OCID`.
<p align="center"><img src="static/oci-screen2.png" alt="Tenancy Information"></p>

- Retorne ao menu Profile, e clique no nome de usuário. Na página de informação do usuário, clique em Copy e salve o `User OCID`.
<p align="center"><img src="static/oci-screen3.png" alt="User Information"></p>

- Agora no canto superior esquerdo, clique no hamburguer menu, vá em `Identity & Security > Identity > Compartments`. Selecione o compartment, clique em Copy e salve o `Compartment OCID`.

<p align="center"><img src="static/oci-screen4.png" alt="Compartment Information"></p>

`Importante: O usuário deverá ter acesso como manage ao compartment selecionado`

- Clique no hamburguer menu, vá em Governance & Administration > Region Management, copie e salve o `Region`.

<p align="center"><img src="static/oci-screen5.png" alt="Region Information"></p>


Lista de ferramentas para pipeline
https://www.lambdatest.com/blog/31-best-ci-cd-tools/

### Contato

[![Twitter Badge](https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white)](https://twitter.com/lucianosilva)
[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/lucianocarmo/)

<p align="center">Copyright © 2022 <a href="https://github.com/lucianosilva">lucianocarmo</a></p>