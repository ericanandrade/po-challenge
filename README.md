# Teste Product Owner - Shipay

### 1) Conheça um pouco mais sobre a hierarquia de cadastro na Shipay:

O cadastro básico de um cliente Shipay consiste em:

**(i)   Conta Shipay:** Conta do lojista cadastrado na Shipay 
 - Dados necessários: nome da conta e email de cadastro

**(ii)  Usuário do Painel Shipay:** permite login no Painel Shipay
- Dados necessários: nome, cpf, telefone, e-mail do usuário e senha

**(iii) Loja:** Necessário para o cliente conseguir gerar cobranças via PIX e carteiras digitais 
- Dados necessários: CNPJ, endereço, nome da loja, quantidade de caixas

---

Atualmente só é possível cadastrar essas entidades separadamente, ou seja, primeiro é necessário cadastrar a **(i) Conta Shipay**, depois deve ser cadastrado o **(ii) Usuário do Painel Shipay** e após, deve ser cadastrada uma **(iii) Loja** na Conta do cliente Shipay. Cada um desses cadastros é feito por um usuário administrador em formulários separados.


Considerando esse cenário, um parceiro estratégico trouxe a seguinte demanda para você, Product Owner da Shipay:


*"Gostaria de ter a possibilidade de cadastrar a **(i) Conta Shipay**, o **(ii) Usuário do Painel Shipay** e uma **(iii) Loja** com um único formulário para não ter que acessar 3 formulários separados para concluir o cadastro do Lojista na Shipay."*


Você entendeu a demanda e pediu auxílio do time de Design de Produto para desenhar uma tela com essa funcionalidade. O time de Design te entregou o seguinte modal de cadastro:

![modal_de_cadastro_completo](https://user-images.githubusercontent.com/59707512/137926227-831000a7-ae66-4b34-80d3-d45fda7f909f.png)


#### Você aprovou o design da tela e deve priorizar essa atividade junto ao time de desenolvimento. Escreva a user-story para essa funcionalidade:
1. OBJETIVO
Unificar os 3 formulários de cadastro de Conta Shipay, Usuário do Painel Shipay e Loja na Conta do cliente Shipay em somente 1 formulário.

2. PREMISSAS
Permitir que o usuário realize as ações de cadastros de Conta, Usuário e Loja em somente uma tela. 

3. REQUISITOS FUNCIONAIS
Atualmente só é possível cadastrar essas entidades separadamente, ou seja, primeiro é necessário cadastrar a (i) Conta Shipay, depois deve ser cadastrado o (ii) 
Usuário do Painel Shipay e após, deve ser cadastrada uma (iii) Loja na Conta do cliente Shipay, acessando 3 formulários distintos. Sendo assim, devemos desenvolver 
a funcionalidade que permita esta ação de realizar todos os cadastros de uma só vez.

4. ESPECIFICAÇÃO FUNCIONAL
Quando um usuário Administrador acessar os "Cadastros" a tela que será aberta apresentará um cadastro completo.
Neste cadastro todos os campos serão obrigatórios.
Os campos CPF, E-mail, Telefone, CNPJ devem checar se os dados digitados são validos. 
Campo CEP, ao preencher já sugere o endereço, porém permite alterar.

---


### 2) O time de desenvolvimento concluiu o desenvolvimento da funcionalidade descrita na questão anterior. Quais testes funcionais você faria para validar essa funcionalidade?
Teste 1 - Verificar se os campos CPF, E-mail, Telefone, CNPJ estão aceitando somente dados válidos.
Teste 2 - Se ao clicar em salvar o processo é confirmado.
Teste 3 - Se o processo é confirmado, verificar se os cadastros de Conta Shipay, Usuário do Painel Shipay e Loja na Conta do cliente Shipay foram criados corretamente
e se os dados foram salvos corretos.
Teste 4 - Testar acessos com dados cadastrados
