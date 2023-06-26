## Projeto Individual - Módulo 3


# Sistema Resilia Data



Este projeto tem como objetivo o desenvolvimento de um banco de dados para o sistema RESILIADATA, que auxilia na avaliação das tecnologias utilizadas pelas empresas parceiras e no registro dos colaboradores.
#
#

O sistema RESILIADATA oferece as seguintes funcionalidades:

## Cadastro de empresas parceiras:

 Permite o registro das informações das empresas parceiras, incluindo nome, endereço, telefone e email.

## Cadastro de tecnologias:

 Permite o registro das tecnologias utilizadas, com a opção de selecionar a área correspondente, como webdev, dados, marketing, etc.

## Registro de tecnologias das empresas:

 Permite associar as tecnologias utilizadas por cada empresa parceira. Essa tabela de relação armazena informações sobre quais tecnologias cada empresa está utilizando.

## Cadastro de colaboradores:

 Permite o registro dos colaboradores, incluindo nome, cargo e a empresa parceira à qual estão vinculados.

## Diagrama

O diagrama mapeado para o banco de dados do projeto RESILIADATA está disponível neste link aqui.

Entidades:

1. Empresa parceira
   - ID 
   - Nome 
   - Endereço 
   - Telefone 
   - Email 

2. Tecnologia
   - ID 
   - Nome 
   - Área 

3. Relação entre Empresa parceira e Tecnologia
   - ID 
   - ID da Empresa parceira (inteiro, chave estrangeira referenciando a tabela Empresa parceira)
   - ID da Tecnologia (inteiro, chave estrangeira referenciando a tabela Tecnologia)

4. Colaborador
   - ID 
   - Nome 
   - Cargo 
   - ID da Empresa parceira (inteiro, chave estrangeira referenciando a tabela Empresa parceira)

## Relacionamentos:

- Uma Empresa parceira pode ter várias Tecnologias associadas a ela.
- Um Colaborador está vinculado a uma única Empresa parceira.
- A tabela de relação entre Empresa parceira e Tecnologia permite registrar quais tecnologias uma empresa está utilizando.

Exemplo de Registros:

Tabela Empresa parceira:
| ID |     Nome     |     Endereço     |   Telefone  |          Email          |
|----|--------------|------------------|-------------|------------------------|
|  1 | Empresa A    | Endereço A       | 123456789   | empresaA@example.com    |
|  2 | Empresa B    | Endereço B       | 987654321   | empresaB@example.com    |

Tabela Tecnologia:
| ID |     Nome     |     Área     |
|----|--------------|--------------|
|  1 | Tecnologia A | WebDev       |
|  2 | Tecnologia B | Dados        |

Tabela Relação Empresa-Tecnologia:
| ID | ID da Empresa parceira | ID da Tecnologia |
|----|-----------------------|-----------------|
|  1 |           1           |        1        |
|  2 |           1           |        2        |
|  3 |           2           |        1        |

Tabela Colaborador:
| ID |    Nome    |     Cargo     | ID da Empresa parceira |
|----|------------|---------------|-----------------------|
|  1 | Colaborador A | Desenvolvedor |           1           |
|  2 | Colaborador B | Analista | 2 

## Perguntas sobre o Mapeamento

Perguntas sobre o mapeamento podem ser consultadas neste link: https://1drv.ms/w/s!Ap-ZYm0t5RTFnQaKGjMCC2Aebeta?e=IW61I9.

## Contato

Jaqueline Cunha 

Email - jakchellyrick@gmail.com

Github - https://github.com/Jaqueline-SPC