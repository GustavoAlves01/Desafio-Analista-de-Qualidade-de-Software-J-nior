# DESAFIO BEEDOO

# User Story

## **Descrição:**
Como um usuário,
Eu quero cadastrar novos cursos através de um formulário,
Para que esses cursos sejam listados na tela de listagem de cursos.

## **Critérios de Aceitação:**
- O sistema deve ter uma tela para listagem de cursos.
- Na tela de listagem de cursos, deve haver um botão para levar à tela de cadastro de cursos.
- O formulário de cadastro de cursos deve conter os seguintes campos obrigatórios: Nome do curso, descrição do curso, instrutor, URL da imagem de capa, data de início, data de fim, número de vagas, tipo de curso (presencial ou online).
- Se o tipo de curso for presencial, um campo para endereço deve ser exibido.
- Se o tipo de curso for online, um campo para o link da inscrição deve ser exibido.
- Todos os campos devem ser obrigatórios e validados corretamente.
- O botão de cadastrar curso deve estar desabilitado até que todos os campos estejam preenchidos corretamente.
- Após o envio bem-sucedido, o curso deve ser listado na tela de listagem de cursos.
- Em caso de erro, uma mensagem de erro apropriada deve ser exibida.

## Decisões Tomadas:

### Análise dos Requisitos do Projeto:
Garantir que a user story cubra todos os aspectos essenciais para a funcionalidade correta do formulário e a integração com a tela de listagem de cursos.

### Entendimento das Necessidades do Usuário:
Facilitar a usabilidade do formulário, garantindo que todos os dados essenciais sejam coletados e exibidos corretamente na tela de listagem.

### Validação dos Campos:
Reduzir erros de entrada de dados e melhorar a qualidade dos dados coletados.

### Acessibilidade e Usabilidade:
Tornar o sistema inclusivo, permitindo que todos os usuários possam utilizá-lo sem barreiras.

## Casos de Teste
[Planilha de Casos de Teste](https://docs.google.com/spreadsheets/d/1Qr71w3px3hI-8yiCwXC1dDrGrHwPp5-AjKKGXFb2R6Y/edit?usp=sharing)

## Passo-a-Passo para Execução dos Casos de Teste

### Caso de Teste 1: Cadastro com sucesso
Passos:
1. Navegue até a tela de cadastro de cursos.
2. Preencha todos os campos corretamente:
3. Clique no botão "Cadastrar".
4. Verifique se o curso foi listado na aba "Listar Cursos".
  Evidência do Teste - [Caso de Teste 1 - Cadastro com Sucesso](https://drive.google.com/file/d/17_yecmiT2vCArfUdKgqiu1Z7gVcwXOrM/view?usp=drive_link)

### Caso de Teste 2: Cadastro com Campos Vazios
Passos:
1. Navegue até a tela de cadastro de cursos.
2. Deixe algum campo obrigatório vazio (por exemplo, "Nome do curso").
3. Clique no botão "Cadastrar".
4. Verifique se o sistema permite o cadastro do curso e se não foi exibida uma mensagem de erro específica para o campo faltante.
  Evidência do Teste - [Caso de Teste 2 - Cadastro com Campos Vazios](https://drive.google.com/file/d/113nUypCKq4MBqKodn5IOKvmhNl7CX-Ax/view?usp=drive_link)

### Caso de Teste 3: Cadastro com Datas Inválidas
Passos:
1. Navegue até a tela de cadastro de cursos.
2. Preencha os campos de data com uma "Data de início" posterior à "Data de fim" (por exemplo, Data de início: "2023-12-31" e Data de fim: "2023-01-01").
4. Clique no botão "Cadastrar".
5. Verifique se o sistema permite o cadastro do curso e se não foi exibida uma mensagem de erro "A data final deve ser posterior à data inicial".
  Evidência do Teste - [Caso de Teste 3 - Cadastro com Datas Inválidas](https://drive.google.com/file/d/1flaJ-C41w77ezAZfxl-ZJXjs8_Nu8rzJ/view?usp=drive_link)

### Caso de Teste 4: Cadastro de Curso com URL Inválida
Passos:
1. Navegue até a tela de cadastro de cursos.
2. Preencha o campo "URL da imagem de capa" com uma URL inválida (por exemplo, "invalid-url").
3. Clique no botão "Cadastrar".
4. Verifique se o sistema permite o cadastro do curso e se não foi exibida uma mensagem de erro "URL da imagem inválida".
  Evidência do Teste - [Caso de Teste 4 - Cadastro de Curso com URL Inválida](https://drive.google.com/file/d/1UtYai5R6L749iQmO60HlIFo3kcTt6Eo0/view?usp=drive_link)

### Caso de Teste 5: Exclusão de Curso
Passos:
1. Navegue até a tela de listagem de cursos.
2. Verifique se existe um curso listado.
3. Clique no botão "Excluir curso" do curso listado.
4. Verifique se o curso não está mais listado na tela de listagem de cursos.
  Evidência do Teste - [Caso de Teste 5 - Exclusão de Curso](https://drive.google.com/file/d/1KH-DO64lvAv_DW-jfiUKYrp14E1Qiiny/view?usp=drive_link)
