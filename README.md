# lista 4 - DER da lista 2 hospital.

| Tabela             | Atributos                                | Chave Primária | Chave Estrangeira |
|--------------------|------------------------------------------|----------------|-------------------|
| Hospital           | Codigo, nome, cidade, estado, bairro, numero, cep, logradouro | Codigo | -                 |
| TelefoneHospital   | NumeroTel, Codigo                       | Codigo (FK) | Codigo (FK)        |
| Paciente           | Num_Identidade, nome, data_de_entrada, data_de_saida | Num_Identidade | -                 |
| Telefone           | num_telefone             | num_telefone | Num_identidade (FK) |
| Tratamento         | Duracao_tratamento | Num_identidade (FK), Matricula (FK) | Num_identidade (FK), Matricula (FK) |
| Profissional       | Matricula, salario, cpf, cargo, nome, dataNascimento | Matricula | Codigo (FK)        |
