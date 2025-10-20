<center>
  <h1 style="font-size:2.4em; margin-bottom:0.1em;">📰 Automação de Resumos de Artigos com n8n</h1>
  <p style="margin-top:0.2em; font-size:1.05em; color:#555;">
    Fluxo automatizado que lê artigos de uma planilha do Google Sheets, gera resumos com IA e envia por e-mail — tudo sem intervenção humana.
  </p>
  <p>
    <a href="https://github.com/Rafael072187/Automacao_de_Resumos_de_Artigos_com_n8n" style="background:#24292F;color:#fff;padding:8px 14px;border-radius:8px;text-decoration:none;font-weight:600;">
      🔗 Repositório no GitHub
    </a>
  </p>
</center>

<hr>

## 🧭 **Tabela de Conteúdos**
- Descrição  
- Instalação  
- Uso  
- Tecnologias  
- Como contribuir  
- Autor  
- Observações  

---

## 📘 **Descrição**
<details>
  <summary><b>Resumo</b></summary>
  Este projeto utiliza o **n8n** para criar uma automação inteligente capaz de:
  - Ler uma lista de links em um **Google Sheets**;
  - Acessar o conteúdo de cada artigo via **HTTP Request**;
  - Extrair o texto em HTML;
  - Gerar **resumos automáticos com IA (OpenAI gpt-4o-mini)**;
  - Enviar o resultado por **e-mail via Gmail API**;
  - Atualizar o status do artigo na planilha como “Resumo já enviado”.

  Ideal para **pesquisadores, jornalistas e profissionais acadêmicos** que precisam processar grandes volumes de links e gerar resumos de forma automática e contínua.
</details>

---

## ⚙️ **Instalação**
<details>
  <summary><b>Passo a passo (Linux / macOS / Windows)</b></summary>

1. Clone o repositório:
   ```bash
   git clone https://github.com/Rafael072187/Automacao_de_Resumos_de_Artigos_com_n8n.git
   cd Automacao_de_Resumos_de_Artigos_com_n8n
Instale o n8n:

bash
Copiar código
npm install -g n8n
Inicie o servidor local:

bash
Copiar código
n8n start
Importe o fluxo Main.json dentro do painel do n8n.

Configure as credenciais necessárias:

Google Sheets API — para ler e atualizar a planilha.

Gmail API — para envio de e-mails.

OpenAI API Key — para geração dos resumos.

HTTP Request — para captura do conteúdo dos artigos.

Certifique-se de ter a planilha configurada com as colunas:

Link do Artigo

Email

Status

</details>
🖥️ Uso
<details> <summary><b>Como usar o projeto</b></summary>
Configure o fluxo no n8n e agende a execução a cada 10 minutos (usando o nó Schedule Trigger).

Insira os links dos artigos na planilha junto com os e-mails de destino.

Quando o fluxo for executado:

Ele lerá a planilha;

Processará os links ainda sem status;

Criará um resumo em 5 tópicos usando a IA da OpenAI;

Enviará o resultado por e-mail;

Atualizará o status na planilha.

</details> <p align="center" style="margin-top:14px;"> <img src="https://cdn-icons-png.flaticon.com/512/9489/9489766.png" width="90" alt="ícone ilustrativo"> <br> <i>Resumo automatizado de artigos com integração Google Sheets + OpenAI + Gmail.</i> </p>
🛠️ Tecnologias
<details> <summary><b>Stack principal</b></summary>
n8n — Automação e orquestração de fluxos

OpenAI GPT-4o-mini — Geração dos resumos

Google Sheets API — Entrada e atualização de dados

Gmail API — Envio automatizado de e-mails

HTTP Request + HTML Parser — Extração de conteúdo dos artigos

</details>
🤝 Como contribuir
<details> <summary><b>Guia rápido</b></summary>
Faça um fork do repositório

Crie uma nova branch:

bash
Copiar código
git checkout -b feature/nova-feature
Realize suas alterações e faça o commit:

bash
Copiar código
git commit -m "feat: adiciona melhoria no processamento de artigos"
Envie as alterações:

bash
Copiar código
git push origin feature/nova-feature
Abra um Pull Request descrevendo sua contribuição.

</details>
👤 Autor
<details> <summary><b>Contatos</b></summary> <p> <b>Rafael Bittencourt de Araújo</b> — desenvolvedor do projeto.<br> GitHub: <a href="https://github.com/Rafael072187" target="_blank">github.com/Rafael072187</a> </p> </details>
📝 Observações
✅ Projeto voltado para automação de resumos acadêmicos e jornalísticos.
🔧 Pode ser expandido para incluir exportação em PDF ou envio em múltiplos idiomas.
⚠️ Garanta que os tokens da OpenAI e Gmail estejam corretamente configurados para evitar falhas no fluxo.

<p align="center" style="margin-top:18px;"> <a href="https://github.com/Rafael072187/Automacao_de_Resumos_de_Artigos_com_n8n" style="background:#0b5fff;color:#fff;padding:10px 18px;border-radius:8px;text-decoration:none;font-weight:600;"> Ver repositório </a> </p> <p align="center" style="margin-top:14px;color:#666;"> Estrutura gerada automaticamente com base no repositório analisado. </p> ```
