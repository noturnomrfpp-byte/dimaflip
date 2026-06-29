# Política de Privacidade — Dimaflip

**Última atualização:** 29/06/2026

---

## 1. Quem somos

O **Dimaflip** é um aplicativo independente com ferramentas de entretenimento e utilitários para jogadores. Esta política explica o que o aplicativo faz (e não faz) com os seus dados.

Esta política foi atualizada para refletir a funcionalidade de **consulta de data de criação de contas por ID**, que utiliza serviços de servidor para funcionar.

---

## 2. Resumo rápido

- **Não há cadastro, login ou conta de usuário.** Não pedimos nome, e-mail, telefone ou senha.
- A maior parte dos seus dados (histórico, favoritos, moedas, progresso) fica **apenas no seu dispositivo**.
- A funcionalidade de **consulta de ID** envia o número de ID digitado aos nossos serviços de servidor (Firebase/Google Cloud) e a uma API pública de terceiros, para retornar a informação pública daquela conta.
- Para evitar abuso dessa funcionalidade, usamos um **identificador técnico do app** (Firebase Installation ID) — ele não identifica você pessoalmente.

---

## 3. Dados que NÃO coletamos

O Dimaflip **não coleta** nem solicita:

- Nome, e-mail, telefone, senha ou qualquer credencial
- Localização (GPS ou aproximada)
- Contatos, fotos, vídeos ou arquivos do dispositivo
- Histórico de navegação ou de outros aplicativos
- Identificadores de publicidade para rastreamento (Advertising ID, IMEI, MAC)
- Dados biométricos

Não há cadastro, login, conta de usuário nem autenticação por dados pessoais no aplicativo.

---

## 4. Dados que ficam apenas no seu dispositivo

Para o aplicativo funcionar, algumas informações são guardadas localmente, no próprio aparelho, usando os mecanismos de armazenamento padrão do Android (Hive e SharedPreferences):

- Histórico de nicks gerados
- Histórico de combinações geradas
- **Histórico das suas consultas de ID** (os IDs consultados e o resultado retornado ficam salvos localmente para sua conveniência)
- Itens favoritados
- Sequência de *check-in* diário
- Progresso de missões e do quiz
- Moedas fictícias internas (sem valor monetário real e não-compráveis)
- Preferências do app (tema escuro/claro, sons, animações)

Esses dados **ficam no seu dispositivo**. Quando você desinstala o aplicativo, todos eles são apagados automaticamente pelo sistema operacional.

---

## 5. Dados processados pela funcionalidade de consulta de ID

A funcionalidade "Data de criação da conta" funciona da seguinte forma:

1. Você digita um **número de ID** de uma conta de jogo.
2. O app envia esse número aos nossos serviços de servidor, hospedados no **Google Firebase / Google Cloud** (região South America).
3. Nosso servidor consulta uma **API pública de terceiros** especializada nesse tipo de informação e retorna dados **públicos** daquela conta: o apelido (nick) e a data de criação.
4. O resultado é exibido para você e salvo no histórico local do seu dispositivo.

**Importante:**

- O ID consultado **pode não ser o seu** — você pode consultar qualquer ID público. Os dados retornados (nick e data de criação) são informações **públicas** fornecidas pela API de terceiros, não dados privados ou sensíveis.
- Para reduzir custos e acelerar respostas, o resultado de uma consulta pode ser **armazenado temporariamente em cache no servidor por até 24 horas**. Esse cache contém apenas o ID consultado e a informação pública retornada (nick e data de criação) — nenhum dado seu.
- Não associamos as consultas à sua identidade pessoal (não há login), apenas a um identificador técnico do dispositivo, descrito na seção 6.

---

## 6. Identificador técnico e prevenção de abuso

Para impedir o uso abusivo da funcionalidade de consulta (por exemplo, um número excessivo de consultas automatizadas que sobrecarregaria o serviço), utilizamos dois mecanismos do Google Firebase:

- **Firebase App Check (Play Integrity):** verifica que as requisições vêm de uma instalação legítima do aplicativo, e não de scripts externos. Esse processo é gerenciado pelo Google.
- **Firebase Installation ID (FID):** um identificador técnico gerado pelo Firebase para cada instalação do app. Usamos esse identificador apenas para aplicar um limite de frequência de consultas por dispositivo. **O FID não contém e não revela dados pessoais seus** (nome, e-mail, etc.) e é redefinido caso o app seja reinstalado ou seus dados sejam limpos.

Esses identificadores são usados **exclusivamente** para segurança e prevenção de abuso, não para publicidade ou rastreamento entre aplicativos.

---

## 7. Permissões solicitadas

O Dimaflip declara a permissão Android **`INTERNET`**, necessária para:

- A funcionalidade de consulta de ID (comunicação com nossos serviços de servidor e a API de terceiros)
- O carregamento de recursos públicos por bibliotecas internas (por exemplo, *Google Fonts*)

Não acessamos câmera, galeria, microfone, contatos, localização, SMS, calendário, sensores biométricos ou qualquer outra permissão sensível do dispositivo.

---

## 8. Serviços de terceiros que utilizamos

Para fornecer a funcionalidade de consulta, o app utiliza:

- **Google Firebase / Google Cloud** (Cloud Functions, Firestore, App Check, Installations) — infraestrutura de servidor e segurança. O tratamento de dados pelo Google é regido pela política de privacidade do Google: https://policies.google.com/privacy
- **API pública de provedor de dados de jogos (terceiro)** — fornece a informação pública de nick e data de criação a partir do ID consultado. Enviamos a esse provedor apenas o número de ID consultado.
- **Google Fonts** — carregamento de tipografia.

Não vendemos, alugamos nem compartilhamos seus dados com terceiros para fins de marketing.

---

## 9. Crianças (menores de 13 anos)

Este aplicativo é destinado a usuários com **13 anos ou mais**. Não coletamos intencionalmente dados de crianças menores de 13 anos. Se você é responsável legal por uma criança que está usando o app e tem dúvidas sobre privacidade, entre em contato pelo e-mail abaixo.

---

## 10. Seus direitos e como apagar seus dados

- **Apagar o histórico de consultas e gerações:** use as opções de "Limpar histórico" dentro do aplicativo.
- **Apagar tudo do dispositivo:** desinstale o aplicativo. Todos os dados locais são removidos pelo sistema operacional.
- **Cache no servidor:** o cache de consultas é temporário (até 24 horas) e expira automaticamente. Ele não está associado à sua identidade pessoal. Caso queira solicitar a remoção de uma entrada específica de cache, entre em contato pelo e-mail abaixo informando o ID.

Em conformidade com a **LGPD (Lei Geral de Proteção de Dados, Lei nº 13.709/2018)**, você tem direito de acesso, retificação e exclusão dos seus dados pessoais. Como não mantemos cadastro nem dados pessoais identificáveis em nossos servidores, o controle dos dados do app está majoritariamente com você, no seu próprio aparelho.

---

## 11. Alterações nesta política

Podemos atualizar esta política eventualmente, por exemplo quando novas funcionalidades forem adicionadas ao aplicativo. Mudanças significativas serão refletidas no campo "Última atualização" no topo desta página e descritas no histórico de versões na Google Play Store.

---

## 12. Contato

Para dúvidas, sugestões ou solicitações relacionadas a privacidade:

📧 **contatodimaflip@gmail.com**

Responderemos em prazo razoável.

---

*Dimaflip é um aplicativo independente de utilitários para jogadores, sem afiliação com qualquer jogo, plataforma ou empresa de terceiros.*
