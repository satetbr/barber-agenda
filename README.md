# Barber Agenda

Aplicativo Android para organizar agendamentos de uma barbearia, com cadastro, consulta e exclusão de horários. O foco é simplicidade de uso e persistência local para funcionar offline.

## Funcionalidades

1. Cadastro de agendamentos com nome, telefone, data e hora.
2. Validação de campos obrigatórios e do telefone com máscara.
3. Consulta de agendamentos com navegação anterior/próximo.
4. Exclusão de agendamentos.
5. Persistência local com SQLite (funciona sem internet).

## Pontos positivos do projeto

1. **UX guiada**: uso de DatePicker/TimePicker e máscara de telefone reduz erros de digitação.
2. **Dados consistentes**: bloqueio de datas passadas e validação de campos essenciais antes de salvar.
3. **Persistência offline**: banco SQLite com ordenação por data/hora facilita a consulta cronológica.
4. **Organização do código**: responsabilidades separadas (UI nas Activities, acesso a dados em `BD`, mensagens em `Msg`).
5. **Navegação clara**: fluxo simples entre telas (home → agendamento → consulta).

## Tecnologias

1. **Android SDK** (Java)
2. **SQLite**
3. **Maskara** (máscara de telefone)

## Estrutura do projeto

1. `MainActivity` — tela inicial.
2. `tela_agendar` — cadastro de agendamentos.
3. `tela_consultar` — consulta, navegação e exclusão.
4. `BD` — criação de tabela e operações no SQLite.
5. `Msg` — diálogo simples de feedback ao usuário.

## Como executar

1. Abra o projeto no **Android Studio**.
2. Aguarde o **Gradle sync**.
3. Execute em um emulador ou dispositivo com **Android 5.0+ (minSdk 21)**.

## Screenshots

||||
|:---:|:---:|:---:|
| ![tela-1](https://github.com/user-attachments/assets/dba28072-bec5-46c6-addb-f43675b8ee04) | ![tela-2](https://github.com/user-attachments/assets/461d713e-4223-476b-afbf-7f0058349aea) | ![tela-3](https://github.com/user-attachments/assets/11a8887f-ddc3-419a-9b50-31fa726689ff) |

||||
|:---:|:---:|:---:|
| ![tela-4](https://github.com/user-attachments/assets/774f8f21-493d-4db2-8d43-e39208b0ebcf) | ![tela-5](https://github.com/user-attachments/assets/21e2ae64-f1f2-4f5f-ac85-266ea9f8dcef) | ![tela-6](https://github.com/user-attachments/assets/0c0b636a-b31b-48a9-8739-45de727cdbcb) |
