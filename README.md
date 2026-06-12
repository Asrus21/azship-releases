# AzShip — Downloads e Atualizações

Repositório oficial de **distribuição do aplicativo AzShip** (arquivos `.apk`).
O código-fonte é mantido em repositório privado; aqui ficam apenas os instaladores
e o histórico de versões.

> Este arquivo é gerado automaticamente a partir do repositório do app. Para
> alterá-lo, edite `releases-readme/README.md` no projeto.

> 📲 **Baixar a versão mais recente:**
> [**Releases → Latest**](../../releases/latest) — baixe o arquivo `azship-XX.apk`
> em **Assets** e instale no celular.

---

## O que é o AzShip

Aplicativo Android para **gestão de motoristas, veículos e documentos** no setor
de transporte de cargas (fretes/logística). Centraliza o cadastro da frota e
**alerta sobre o vencimento de documentos** (CNH, CRLV, etc.), reduzindo multas e
bloqueios por irregularidade.

- **Plataforma:** Android 14 ou superior
- **Acesso por perfil:** Motorista, Administrativo e Master

## Funcionalidades

- **Cadastro de motoristas** (nome, CPF, CNH e categoria, telefone, e-mail,
  endereço, situação)
- **Cadastro de veículos** por motorista (placa, marca, modelo, ano, cor,
  RENAVAM, tipo)
- **Cadastro de documentos** por motorista (tipo, número, validade, descrição)
- **Alertas de vencimento** de documentos (vencido / vence em ≤30 dias / em dia)
- **Resumo no painel** com contadores e **busca/filtros** de motoristas
- **Login por perfil** com senha protegida e **token de ativação** para motoristas
- **Exportar lista (CSV)** e **compartilhar ficha** do motorista
- **Ligar / WhatsApp** direto na ficha do motorista
- **Atualização dentro do app**: aviso automático quando há uma versão nova

## Como instalar

1. Abra a [**última release**](../../releases/latest) no navegador do celular.
2. Em **Assets**, baixe o arquivo `azship-XX.apk`.
3. Toque no arquivo baixado para instalar (na primeira vez, o Android pede para
   **permitir instalar de fontes desconhecidas** — é um ajuste único).

## Como atualizar

- O próprio app avisa **"Nova versão disponível"** ao abrir, com um botão para
  baixar a atualização.
- Como é a mesma assinatura, a nova versão **instala por cima** sem perder dados.

## Requisitos

- Android **14 (API 34)** ou superior.

---

## Histórico de versões (changelog)

> As versões abaixo são as **liberações oficiais**. Builds de teste, geradas
> manualmente apenas para validação, **não são listadas aqui** (elas podem
> aparecer na aba *Releases*, mas não fazem parte do changelog).

### 1.0.27 — Nova navegação
- **Menu lateral** (☰) e **barra inferior** para navegar pelas seções.
- Painel mais limpo, com o resumo da frota em destaque.

### 1.0.26 — Atualização automática no app
- Tocar em **Atualizar** baixa o APK e abre o instalador **dentro do app**
  (sem ir ao GitHub/navegador); basta confirmar "Instalar".

### 1.0.25 — Conta principal fixa
- A **conta principal** do sistema é fixa: sempre existe e não pode ser
  alterada nem excluída.

### 1.0.24 — Acabamento visual
- **Modo escuro** (acompanha o tema do aparelho).
- **Avisos internos**: comunicados do admin visíveis a todos os usuários.

### 1.0.23 — Segurança e auditoria
- **Log de auditoria** (quem fez o quê e quando), consultável pelo Master.
- **Bloqueio do login** após 5 tentativas erradas.
- **"Esqueci minha senha"** com token de redefinição gerado pelo admin.
- **Biometria/PIN ao abrir o app** (opcional).

### 1.0.22 — Módulo de Viagens
- **Cadastro de viagens/fretes** com motorista e veículo vinculados.
- **Status** (Agendada → Em andamento → Concluída) com checklist de saída.
- **Despesas por viagem** com total calculado.
- Motorista vê e movimenta **as próprias viagens**.

### 1.0.21 — Relatórios e PDF
- **Ficha do motorista em PDF** e **relatório de vencimentos em PDF**.
- **Tela de Relatórios** com números da frota.

### 1.0.20 — Identidade do motorista
- **Foto de perfil do motorista** no cadastro, na lista e na ficha.
- **Carteirinha digital** com foto, dados e **QR code**.
- Motorista pode **editar os próprios contatos**.

### 1.0.19 — Robustez
- Consultas ao banco em segundo plano (sem travamentos com muitos registros).
- Confirmação ao sair de formulários com alterações não salvas.
- **"Desfazer"** ao excluir veículos e documentos.

### 1.0.18 — Changelog no app e verificação de atualização
- O histórico de novidades passa a ser exibido **dentro do app** (em cards).
- "Verificar atualização" avisa quando **já está na versão mais recente**.

### 1.0.17 — Fotos, notificações, backup e configurações
- **Foto anexada ao documento** (câmera ou galeria) com visualização em tela cheia.
- **Notificação de vencimento com o app fechado**: verificação diária que avisa
  quando há documentos vencidos ou vencendo.
- **Backup e restauração** dos dados em arquivo (restauração exclusiva do Master).
- **Tela de Configurações**: antecedência do alerta (7/15/30 dias) e seção
  **Sobre** (versão instalada, novidades e verificação de atualização).

### 1.0.15 — Seletores e validação
- **Tipo de documento** agora é selecionável (CNH / RG), em vez de digitado.
- **Categoria da CNH** agora é selecionável (A, B, AB, C, D, E, AC, AD, AE, ACC).
- **Validação de e-mail** no cadastro de motorista.

### 1.0.13 — Login e senha
- Aviso de **nova versão também na tela de login**.
- **Botão "olho"** para mostrar/ocultar a senha nos campos de senha.

### 1.0.11 — Token de ativação rotativo
- O **token de ativação** do motorista passa a **mudar a cada 10 minutos**.
- Após ativar, o acesso permanece no aparelho até desinstalar/limpar os dados.

### 1.0.9 — Distribuição pública
- APKs passam a ser publicados neste repositório público, mantendo o código
  privado. Aviso de atualização dentro do app.

### 1.0 — Versão inicial
- Cadastro de motoristas, veículos e documentos; perfis de acesso; alertas de
  vencimento; busca, filtros e contadores; exportação CSV; compartilhar ficha;
  ligar/WhatsApp; build e publicação automatizados.

---

<sub>Para manutenção: ao publicar uma versão real, adicione uma entrada acima com
o número da versão e as novidades. Não inclua builds de teste.</sub>
