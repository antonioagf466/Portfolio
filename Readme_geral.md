# ⚙️ Automações e Fluxos — AGERGS

Além dos projetos detalhados neste portfólio, desenvolvi uma **coleção de fluxos e automações no Power Automate**. Eles foram criados para **economizar tempo, reduzir tarefas repetitivas e deixar a rotina de trabalho mais simples**, tanto para o setor de TI quanto para a AGERGS como um todo.

![Visão geral](/fluxos_pad.png)
---

## 🎯 Objetivo

Muitas atividades do dia a dia eram feitas à mão: consultar sites, baixar e ler documentos, copiar informações para planilhas, conferir prazos e avisar pessoas. Cada fluxo desta lista nasceu de uma dessas necessidades. A ideia é que o trabalho repetitivo fique com a máquina, e as pessoas usem o tempo na parte que exige análise e decisão.

---

## 🗂️ Fluxos por categoria

| Categoria | Fluxos | Para que servem |
|---|---|---|
| **Extração de dados** | `DTI - Extrator - TCE - Licitacon` · `DTI - Extrator DOE RS` · `DTI - Extrator - PDF do Diário dos Municípios` | Coletam automaticamente informações de fontes públicas: LicitaCon (TCE-RS), Diário Oficial do Estado e Diário dos Municípios |
| **Contratos** | `Renovacao_Contrato_DOE` | Identifica nas publicações do Diário Oficial as renovações de contratos e atualiza o painel de contratos |
| **Senhas** | `DTI - Senhas` · `ProjetoDTI - Senhas` | Avisam no Teams, **10 dias antes**, que a senha de rede (AD) vai expirar, para a pessoa trocar a tempo |
| **Senhas administrativas** | `DTI - Senhas Administrativas` · `ProjetoDTI - Senhas Administrativas` | Mesmo aviso de expiração, aplicado às contas administrativas |
| **Tratamento especial** | `DTI - Tratamento Especial` · `ProjetoDTI - Tratamento Especial` | Cobrem as pessoas que fogem da regra padrão do AD e por isso não entram no fluxo normal de aviso de senha |
| **Alertas DTM** | `Alertas DTM` · `ProjetoDTI - Alertas DTM` | Avisam empresas que têm documentos a enviar e que o prazo está perto de vencer |

---

## 🔗 Onde essas automações aparecem no portfólio

Alguns desses fluxos alimentam os outros projetos:

| Projeto | Fluxos que alimentam |
|---|---|
| **Dashboard Diário Oficial** | `DTI - Extrator DOE RS` coleta as publicações exibidas no painel |
| **Análise dos Contratos** | `DTI - Extrator - TCE - Licitacon` traz os dados dos contratos, e `Renovacao_Contrato_DOE` atualiza as renovações a partir do que sai no Diário Oficial |
| **Sistema de Chamados da DTI** | Automação separada, feita com Forms, SharePoint e Teams |

---

## 💡 Impacto

| Área | O que as automações entregam |
|---|---|
| **Todos os servidores** | Aviso de expiração de senha com antecedência, o que evita bloqueio de acesso no meio do expediente |
| **Setor de TI** | Menos trabalho manual com avisos, coleta de dados e acompanhamento |
| **Contratos e publicações** | Informações do DOE e do LicitaCon sempre atualizadas, sem copiar dados à mão |
| **Relacionamento com empresas** | Alertas de prazo para envio de documentos, sem depender de lembrança manual |

---

## 🛠️ Tecnologias

| Ferramenta | Uso |
|---|---|
| Power Automate Desktop | Automação de tarefas em sites, arquivos e aplicativos |
| Power Automate Cloud | Integração com Forms, SharePoint, Teams e Excel |
| Active Directory (AD) | Origem dos dados de expiração de senha |
| Microsoft Teams | Canal dos avisos para as pessoas |
| Excel / CSV / JSON | Saída e armazenamento dos dados coletados |
| Power BI | Visualização dos dados gerados pelas automações |

---

## 📚 Aprendizados

- Identificar tarefas repetitivas que valem a pena automatizar.
- Extrair informações de **sites e PDFs** de forma estruturada.
- Criar **avisos preventivos** que evitam problemas, como a senha que expira sem ninguém perceber.
- Tratar **exceções à regra padrão**, como as contas com política própria no AD.
- Organizar os fluxos com **nomes padronizados**, para facilitar a manutenção.
- Reaproveitar a mesma automação em mais de um projeto.

---

## 👤 Autor

**Antonio Augusto Geraldes Filho**
Estagiário de Dados/TI na AGERGS · Análise e Desenvolvimento de Sistemas, Senac-RS
📍 Porto Alegre, RS
