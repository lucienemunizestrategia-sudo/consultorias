# Formulario de Cadastro - Prospera Rio

Sistema de cadastro online para o programa Prospera Rio, conectado a planilha do Google Sheets.

**Territorios:** Mare . Jacarezinho

---

## Arquivos

| Arquivo | Descricao |
|---------|-----------|
| `index.html` | Formulario HTML completo com CSS e JavaScript |
| `webapp-code.js` | Codigo a ser adicionado no Google Apps Script |

---

## Instalacao

### Passo 1: Configurar o Google Apps Script

1. Abra sua planilha:
   https://docs.google.com/spreadsheets/d/1uWeG39Yxw3pxlYCTWyKKKltduot5mCMF98LAa_9JlFk/edit

2. Va em **Extensoes** > **Apps Script**

3. No arquivo `Code.gs`, **ADICIONE** o codigo do arquivo `webapp-code.js` ao **FINAL** do codigo existente
   - NAO substitua o codigo atual, apenas adicione ao final

4. Salve o projeto (Ctrl + S)

### Passo 2: Implantar como Web App

1. No Apps Script, clique em **Implantar** > **Nova implantacao**

2. Configure assim:
   - **Tipo:** App da Web
   - **Descricao:** Formulario Cadastro
   - **Executar como:** Eu (sua conta)
   - **Quem pode acessar:** Qualquer pessoa

3. Clique em **Implantar**

4. Autorize as permissoes quando solicitado

5. **COPIE a URL do Web App** que sera exibida
   - Exemplo: `https://script.google.com/macros/s/AKfycbx.../exec`

### Passo 3: Atualizar o Formulario HTML

1. Abra o arquivo `index.html`

2. Encontre a linha:
   ```javascript
   const WEBAPP_URL = 'SUA_URL_DO_WEBAPP_AQUI';
   ```

3. Substitua pela URL que voce copiou:
   ```javascript
   const WEBAPP_URL = 'https://script.google.com/macros/s/AKfycbx.../exec';
   ```

### Passo 4: Publicar no GitHub Pages

1. Crie um repositorio no GitHub (publico)

2. Faca upload do arquivo `index.html`

3. Va em **Settings** > **Pages**

4. Em **Source**, selecione:
   - **Branch:** main
   - **Folder:** / (root)

5. Clique em **Save**

6. Sua pagina estara disponivel em:
   `https://SEU_USUARIO.github.io/NOME_DO_REPO/`

---

## Funcionalidades

- Cadastro de Pessoa Fisica (CPF)
- Cadastro de Pessoa Juridica (CNPJ)
- Campos de Data e Horario do atendimento
- Lista completa de Eventos/Consultorias
- Validacao de CPF e CNPJ
- Mascaras de formatacao
- Design responsivo
- Integracao automatica com Google Sheets

---

## Campos do Formulario

### Pessoa Fisica (24 colunas)
1. Data
2. Horario Inicio
3. Horario Fim
4. Nome
5. CPF
6. Sexo
7. Nascimento
8. Tipo de Logradouro
9. Logradouro
10. Numero
11. Complemento
12. Bairro
13. Municipio
14. UF
15. CEP
16. Tipo de Endereco
17. DDD
18. Telefone
19. Complemento Telefone
20. Tipo de Telefone
21. E-mail
22. Tipo de E-mail
23. Ocupacao
24. EVENTO

### Pessoa Juridica (28 colunas)
1. Data
2. Horario Inicio
3. Horario Fim
4. Razao Social
5. CNPJ
6. Data de Fundacao
7. Tipo de Logradouro
8. Logradouro
9. Numero
10. Complemento
11. Bairro
12. Municipio
13. UF
14. CEP
15. DDD
16. Telefone
17. Complemento Telefone
18. Tipo de Telefone
19. E-mail
20. Tipo de E-mail
21. CPF do Contato
22. Nome do Contato
23. Cargo do Contato
24. Nascimento
25. Sexo
26. Classificacao da Empresa
27. CNAE
28. EVENTO

---

## Lista de Eventos

- Consultoria em Diagnostico Empresarial
- Consultoria em Precificacao
- Consultoria de Como Fazer o Instagram
- Consultoria de Cadastro no TikTok
- Consultoria de Sistema de Caixa
- Consultoria de Controle de Estoques
- Consultoria de Entrega de Relatorios
- Consultoria de Como Vender Mais
- Consultoria de Como Lucrar Mais
- Consultoria de Instalacao de Cadastro de Lojas na Shopee
- Consultoria de Cadastro no Google Meu Negocio
- Consultoria de Cadastro no Mercado Livre
- Consultoria de Como Gerir Melhor Seu Negocio
- Consultoria de Coloque Seu Negocio nas Redes Sociais
- Consultoria de Como Digitalizar Seu Negocio
- Consultoria de Como Vender Mais pelo TikTok
- Consultoria de Como Fidelizar Clientes
- Consultoria de Estudo de Caso da Lacoste
- Consultoria em Estrategias de Crescimento

---

## Paleta de Cores

| Cor | Codigo | Uso |
|-----|--------|-----|
| Azul Principal | #092040 | Fundo dos titulos |
| Azul Secundaria | #00B7D7 | Destaques |
| Amarelo Acento | #ECC203 | Botoes |
| Cinza Neutro | #EFF1F3 | Fundos claros |
| Azul Escuro | #021738 | Textos |

---

Prospera Rio - SEBRAE
Mare . Jacarezinho
