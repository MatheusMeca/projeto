# Universidade Estelar
### GRUPO 30
Nós da Universidade desenvolvemos os seguintes protótipos:
### Diagrama de classe
Nosso diagrama de classes é formado por 8 tabelas, sendo elas:
* Banco;
* Usuário;
* Pessoa Física;
* Pessoa Jurídica;
* Aluno;
* Professor;
* Fornecedores;
* Universidade;

A imagem a baixo retrata nosso diagrama:
![diagrama de classe](https://raw.githubusercontent.com/MatheusMeca/projeto/refs/heads/master/documentacao/uml/diagrama_de_classe.jpg)

### Casos de uso:
Nossos casos de uso são:

Cenário Principal para **Aluno**:

* O usuário escolhe a opção “Aluno”.
O sistema exibe a tela de opções:
Fazer login
Criar senha
Informar renda
Solicitar matrícula
Informar número da matrícula
Informar nível de curso desejado
Pagar matrícula
Informar tipo de conta
Consultar frequência
O usuário escolhe a opção “Fazer login”.
O sistema solicita email e senha.
O usuário insere dados incorretos.
O sistema verifica o registro.
Existe, mas os dados estão incorretos.
O sistema retorna “Email ou senha incorretos”.
O usuário insere os dados corretamente.
O sistema verifica o registro.
Existe.
O sistema retorna sucesso.

---
* Cenário Secundário:
O usuário escolhe a opção “Aluno”.
O sistema exibe a tela de opções:
Fazer login
Criar senha
Informar renda
Solicitar matrícula
Informar número da matrícula
Informar nível de curso desejado
Pagar matrícula
Informar tipo de conta
Consultar frequência
O usuário escolhe a opção “Pagar matrícula”.
O sistema solicita forma de pagamento.
O usuário informa a forma de pagamento.
O sistema analisa a forma de pagamento.
Forma de pagamento inválida, tente novamente.
O usuário insere nova forma de pagamento.
O sistema analisa a nova forma de pagamento.
Forma de pagamento válida.
O sistema retorna “Pagamento efetuado com sucesso”.
---

* Cenário Secundário:
O usuário escolhe a opção “Aluno”.
O sistema exibe a tela de opções:
Fazer login
Criar senha
Informar renda
Solicitar matrícula
Informar número da matrícula
Informar nível de curso desejado
Pagar matrícula
Informar tipo de conta
Consultar frequência
O usuário escolhe a opção “Consultar frequência”.
O sistema solicita os dados de matrícula do usuário.
O usuário insere os dados de matrícula.
O sistema analisa os dados de matrícula.
Dados de matrícula inválidos, tente novamente.
O usuário insere os dados de matrícula corretamente.
O sistema analisa os dados de matrícula.
Dados válidos.
O sistema retorna a frequência do usuário.
Pré-condição:
O usuário deve estar registrado no sistema como Aluno.
Pós-condição:
O aluno terá acesso ao seu perfil e poderá consultar suas informações acadêmicas.
---

* Cadastro de Pessoa Jurídica:
Cenário Principal:
O usuário escolhe o tipo de cadastro “Pessoa Jurídica”.
O sistema exibe a tela de opções:
Informar CNPJ
Informar número de matrícula (se aplicável)
Informar o tipo de empresa
Informar área de atuação
Informar o tipo de CNPJ
O usuário escolhe a opção “Informar CNPJ”.
O sistema valida o CNPJ.
CNPJ correto.
O sistema retorna sucesso e permite continuar com o cadastro.
Pré-condição:
O usuário deve ter um CNPJ válido.
Pós-condição:
A empresa estará cadastrada no sistema e poderá acessar as funcionalidades disponíveis.
---

* Cadastro de Pessoa Física:
Cenário Principal:
O usuário escolhe o tipo de cadastro “Pessoa Física”.
O sistema exibe a tela de opções:
Cadastrar pessoa física
Informar número de registro
Informar o tipo de cadastro
Informar se é responsável por algum aluno
Informar CPF
Informar RG
Informar dependente
O usuário escolhe a opção “Cadastrar pessoa física”.
O sistema solicita informações do funcionário.
O usuário insere os dados do funcionário.
O sistema solicita o tipo de contratação.
O usuário insere o tipo de contratação.
O sistema valida os dados e conclui o cadastro.
Cenário Alternativo:
O usuário escolhe a opção “Informar se é responsável por algum aluno”.
O sistema solicita o número de matrícula do aluno.
O usuário insere o número de matrícula do aluno.
O sistema pede o grau de parentesco.
O usuário insere o grau de parentesco.
O sistema valida os dados e conclui a ação.
Pré-condição:
O usuário deve estar registrado no sistema como Pessoa Física.
Pós-condição:
A pessoa física estará cadastrada e, se for responsável por um aluno, essa informação será registrada.
---

* Cadastro de Professor:
Cenário Principal:
O usuário escolhe o tipo de cadastro “Professor”.
O sistema exibe a tela de opções:
Informar nível de graduação
Informar curso a lecionar
Informar matéria a lecionar
Fazer login
Criar senha
Informar salário
Informar CPF/CNPJ
Informar RG
Consultar grade curricular
Consultar notas dos alunos
Consultar provas
Visualizar aulas
Consultar perfil do aluno
O usuário escolhe a opção “Fazer login”.
O sistema solicita email e senha.
O usuário insere dados incorretos.
O sistema verifica o registro.
Existe, mas os dados estão incorretos.
O sistema retorna “Email ou senha incorretos”.
O usuário insere os dados corretamente.
O sistema verifica o registro.
Existe.
O sistema retorna sucesso.
Pré-condição:
O usuário deve ter sido previamente cadastrado como Professor.
Pós-condição:
O professor terá acesso às funcionalidades acadêmicas e administrativas.
---

* Cadastro de Fornecedor:
Cenário Principal:
O usuário escolhe o tipo de cadastro “Fornecedor”.
O sistema exibe a tela de opções:
Cadastrar fornecedores
Criar cadastro
Informar ramo de atuação
Criar senha
Fazer login
Informar CNPJ
Informar endereço
Informar tipo de produto
Consultar agendamentos
O usuário escolhe “Criar cadastro”.
O sistema solicita os dados.
O usuário insere os dados.
O sistema verifica se a conta já existe.
Sim: “Essa conta já existe”.
Não: O sistema retorna “Cadastro criado com sucesso”.
Cenário Alternativo:
O usuário escolhe a opção “Criar senha”.
O sistema solicita os dados da conta.
O usuário insere os dados.
O sistema verifica os dados.
Dados corretos: O usuário cria a senha.
O sistema valida a senha e retorna “Senha criada com sucesso”.
Dados incorretos: O sistema retorna “Dados não encontrados”.
Pré-condição:
O usuário deve fornecer um CNPJ válido.
Pós-condição:
O fornecedor estará registrado e poderá acessar as funcionalidades do sistema.
---

_Abaixo está a nosso diagrama dos casos de uso:_

![](https://raw.githubusercontent.com/MatheusMeca/projeto/refs/heads/master/documentacao/uml/os_casos_de_uso.jpg)

### Também desenvolvemos os prótotipos da telas de cadastro, onde deve ser necessário a seleção do tipo de cadastro à ser realizado:

Tela de seleção de cadatro:


![tela inicial](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_3.png?token=GHSAT0AAAAAAC223IZUZEAMY5LAEBU4NZPQZ2CAMTQ)

### Cadastro Aluno:

![cadastro calouro](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_4.png?token=GHSAT0AAAAAAC223IZU6NQTZLTQVPLBK3MWZ2CANZQ)

### Cadastro de novo Fornecedor:

![cadastro fornecedor](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_5.png?token=GHSAT0AAAAAAC223IZVUXANENXTUAW6R72YZ2CAO2A)

### Cadastro Pessoa Física:

![cadastro pf](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_6.png?token=GHSAT0AAAAAAC223IZVCVGVHUGMCJAPZ76OZ2CAFZA)

### Cadastro Pessoa Jurídica: 

![cadastro pj](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_8.png?token=GHSAT0AAAAAAC223IZUBAK3TM4BVSPSNYTKZ2CAHKA)

### Cadastro Professor:

![cadastro professor](https://raw.githubusercontent.com/9UJAO6/senac/refs/heads/main/Screenshot_7.png?token=GHSAT0AAAAAAC223IZVO3DLVJ7VNTDVKCKMZ2CAGYA)


