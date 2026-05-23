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
| ![tela-1](https://github.com/satetbr/Barber-Agenda/assets/156530052/318091a2-c905-4b3e-af8b-10f0cf3625f4) | ![tela-2](https://github.com/satetbr/Barber-Agenda/assets/156530052/524d0e3d-fac9-4e34-bb3e-5f0b6b471d00) | ![tela-3](https://github.com/satetbr/Barber-Agenda/assets/156530052/ef2b4207-59a2-4404-ab99-20f49055e9bd) |

||||
|:---:|:---:|:---:|
| ![tela-4](https://github.com/satetbr/Barber-Agenda/assets/156530052/6de628c1-2108-4dc7-926e-de4ea8312701) | ![tela-5](https://github.com/satetbr/Barber-Agenda/assets/156530052/ba8d4ff4-3066-4dcb-baa4-148f598d50ce) | ![tela-6](https://github.com/satetbr/Barber-Agenda/assets/156530052/b53df8bb-68d3-4e55-89f5-3e6d03d94192) |
