
# Passo a passo: Como inserir metadados no DSpace

Este guia descreve, passo a passo, como **criar um novo campo de metadado no DSpace** utilizando a interface administrativa.

----------

## 1. Acessar o DSpace como administrador

1.  Abra o DSpace no navegador.
    
2.  Faça login com uma conta que possua **perfil de administrador**.
    

----------

## 2. Acessar o menu de administração

1.  Após o login, localize a **barra lateral** do DSpace.
    
2.  Clique nela 
    

> 📸 **Imagem sugerida:** Barra superior com o menu Administração destacado

----------

## 3. Navegar até a área de metadados

No menu administrativo:

1.  Clique em **Registros**.
    
2.  Em seguida, clique em **Metadados**.
    

Isso abrirá a página de gerenciamento de esquemas e campos de metadados.

> 📸 **Imagem sugerida:** Menu Administração → Registros → Metadados

----------

## 4. Selecionar o esquema de metadados

1.  Na página de metadados, localize a opção para **selecionar o esquema**.
    
2.  Escolha o esquema desejado.
    
    Exemplo:
    
    -   `dublin core`
        
    -   `local`
        
    -   outro esquema personalizado
        

> ℹ️ O esquema **Dublin Core** (`dc`) é o mais utilizado por padrão no DSpace.

> 📸 **Imagem sugerida:** Lista ou seletor de esquemas de metadados

----------

## 5. Criar um novo campo de metadado

Após selecionar o esquema:

1.  Clique no botão **Criar campo de metadado**.
    
2.  Um formulário será exibido para preenchimento dos dados do novo metadado.
    

> 📸 **Imagem sugerida:** Botão "Criar campo de metadado"

----------

## 6. Preencher os dados do metadado

No formulário de criação, preencha os seguintes campos:

### 🔹 Elemento *

-   Campo **obrigatório**.
    
-   Representa o nome principal do metadado.
    

Exemplo:

```
subject

```

----------

### 🔹 Qualificador

-   Campo **opcional**.
    
-   Serve para especializar o elemento.
    

Exemplos:

```
cnpq
por
lattes

```

> ℹ️ Se deixado em branco, o metadado será apenas `dc.element`.

----------

### 🔹 Nota de Escopo

-   Campo **opcional**.
    
-   Usado para descrever a finalidade do metadado.
    
-   Ajuda administradores e catalogadores a entenderem como o campo deve ser usado.
    

Exemplo:

```
Área do conhecimento segundo a classificação do CNPq

```

> 📸 **Imagem sugerida:** Formulário de criação de campo de metadado preenchido

----------

## 7. Salvar o metadado

1.  Após preencher os campos, clique em **Salvar**.
    
2.  O novo metadado passará a fazer parte do esquema selecionado.
    

> 📸 **Imagem sugerida:** Botão Salvar destacado

----------

## 8. Uso do metadado

Após criado:

-   O metadado poderá ser utilizado:
    
    -   Em **formulários de submissão**
        
    -   Em **configurações de busca e facetas (Discovery/Solr)**
        
    -   Em **exibição de itens**
        

> ⚠️ Dependendo do caso, pode ser necessário:

-   Limpar cache
    
-   Reindexar o Solr
    
-   Ajustar o submission form
    

----------

## 📌 Exemplo final de metadado

```
Esquema: dc
Elemento: subject
Qualificador: cnpq
Resultado: dc.subject.cnpq

```

----------

✅ Pronto! O metadado foi criado com sucesso e já pode ser integrado às demais configurações do DSpace.
