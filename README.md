# Agente_Ocorrencias
Agente de IA para automação de relatários operacionais de Mal Súbito

# 🚨 Agente de Ocorrências — Terminal

Gerador inteligente de relatórios de mal súbito para terminais de transporte público. Desenvolvido em HTML puro, roda diretamente no navegador sem necessidade de instalação.

---

## 📋 Sobre o Projeto

O sistema guia o operador por um formulário passo a passo e, ao final, utiliza **Inteligência Artificial** (Groq — LLaMA 3.3 70B) para redigir automaticamente um relatório institucional completo, no mesmo padrão utilizado na operação do terminal.

**Exemplo de relatório gerado:**

> Por volta das 02h04, o Sr. Alexsandro Santos Machado, portador do RG nº 58.611.002-1, foi identificado após sofrer uma queda na Plataforma 03, próximo ao PMD 38. O usuário recebeu auxílio do Vigilante Alexandre Pereira, RE 4520, e do OTU Francisco Santos, RE 266...

---

## ✨ Funcionalidades

- **Formulário guiado** em 5 etapas com validação de campos obrigatórios
- **Geração de relatório por IA** no padrão institucional do terminal
- **Campo de nome do terminal** salvo automaticamente no navegador
- **Histórico de ocorrências** armazenado localmente — consulte, visualize e exclua registros anteriores
- **Exportar para PDF** com cabeçalho formatado
- **Copiar texto** com um clique para colar em qualquer editor
- **100% offline** após carregamento — só precisa de internet para chamar a IA

---

## 📝 Campos do Formulário

| Etapa | Dados coletados |
|---|---|
| Dados do Usuário | Nome, RG, CPF, idade, horário, local, como foi identificado |
| Estado Clínico | Situação, sinais vitais, consciência, cadeira de rodas, aceite de condução, hospital |
| Equipe de Atendimento | Vigilantes, OTUs, CAMs — nome e RE |
| SAMU | Protocolo, atendente, placa, prefixo, equipe médica com RE/CREA |
| Desfecho & Cientes | Horário de finalização, observações, E.T./Supervisão cientes |

---

## 🚀 Como Usar

### Opção 1 — Arquivo local
1. Baixe o arquivo `agente-ocorrencias.html`
2. Dê dois cliques para abrir no navegador (Chrome ou Edge recomendados)

### Opção 2 — GitHub Pages (recomendado)
Acesse diretamente pela URL pública do projeto sem precisar baixar nada.

---

## 🔑 Configuração da Chave de IA

O sistema utiliza a API do **Groq**, que é **gratuita**.

1. Acesse [console.groq.com/keys](https://console.groq.com/keys)
2. Crie uma conta (pode usar login com Google)
3. Clique em **"Create API Key"**
4. Copie a chave gerada (começa com `gsk_...`)
5. Cole no campo que aparece na primeira abertura do sistema

> A chave fica salva no navegador — não é necessário inserir novamente.

---

## 🌐 Publicando no GitHub Pages

1. Suba o arquivo `agente-ocorrencias.html` no repositório
2. Vá em **Settings → Pages**
3. Em **Source**, selecione `main` e clique em **Save**
4. Em alguns minutos o sistema estará disponível em:

```
https://seu-usuario.github.io/nome-do-repositorio
```

> Cada usuário precisará inserir sua própria chave do Groq na primeira vez que acessar.

---

## 🛠️ Tecnologias Utilizadas

| Tecnologia | Uso |
|---|---|
| HTML5 + CSS3 | Interface e estilo |
| React 18 (via CDN) | Componentes e estado da aplicação |
| Babel Standalone | Transpilação JSX no navegador |
| Groq API | Geração de texto com IA (LLaMA 3.3 70B) |
| LocalStorage | Histórico e configurações salvas no navegador |

---

## 📁 Estrutura do Projeto

```
agente-ocorrencias/
│
├── agente-ocorrencias.html   # Aplicação completa (arquivo único)
└── README.md                 # Este arquivo
```

---

## 👤 Autor

Desenvolvido por **Francisco** — estudante de Programação Orientada a Objetos na UniFECAF.

---

## 📄 Licença

Este projeto é de uso livre. Sinta-se à vontade para adaptar para o seu terminal.
