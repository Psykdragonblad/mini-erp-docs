# Requisitos Funcionais - Mini ERP

## RF01 - Cadastro de Produtos
**Como** gestor do estoque,  
**Quero** poder cadastrar novos produtos informando nome, preço e quantidade em estoque,  
**Para** que eu possa controlar o inventário da minha loja.  

### Critérios de Aceite:
1. O campo **Nome** é obrigatório e não pode exceder 100 caracteres.
2. O campo **Preço** deve ser obrigatório e aceitar apenas valores numéricos **maiores que zero** (`> 0`).
3. O campo **Quantidade em Estoque** deve ser obrigatório e aceitar apenas números inteiros **maiores ou iguais a zero** (`>= 0`).
4. Se qualquer validação falhar, a API deve retornar HTTP 400 com a mensagem descritiva do erro.