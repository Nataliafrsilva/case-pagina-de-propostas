# 🚀 Case de Portfólio (TL;DR): Página de Propostas Interativa & Checkout Omnichannel — Aqui Ads (Globo & Eletromidia)

> **Cargo:** Product Manager (PM) responsável pela iniciativa ponta a ponta  
> **Produto:** **Aqui Ads** (Joint Venture / Parceria Estratégica **Globo + Eletromidia** para PMEs)  
> **Escopo:** Discovery, Arquitetura de Regras de Negócio, UX/Checkout B2B, Mobile-First & Prototipação Funcional  
> **Protótipo Navegável:** [Página de Propostas Interativa (Live Demo)](./index.html)

---

## ⚡ 1. TL;DR (Resumo em 30 segundos)

* **O Contexto:** No **Aqui Ads**, propostas comerciais multicanal (*Telas em Elevadores/OOH, Portais Globo & Globoplay, Revistas Digital e Rádio CBN*) precisavam deixar de ser documentos estáticos para se tornarem **máquinas de conversão self-service**.
* **O Problema:** PMEs enfrentavam fricção para entender o valor de múltiplos canais combinados, cadastrar dados de faturamento, aprovar propostas no celular e compartilhar o plano internamente via WhatsApp/e-mail sem travar no tamanho do arquivo ou em regras fiscais distintas entre veículos.
* **O Que Eu Fiz:** Como **Gerente de Produto**, liderei o redesenho estratégico da **Página de Propostas & Checkout**, unificando a apresentação consultiva do plano de mídia (com mapa interativo de pontos OOH e detalhamento de métricas por canal) a um **checkout transparente** que separa o pagamento imediato do faturamento pós-reserva de Rádio.
* **O Resultado:** Redução de **98,4% no peso do PDF executivo** (`18,77 MB` $\rightarrow$ `0,30 MB` para envio instantâneo no WhatsApp), eliminação da fricção de cadastro com **preenchimento progressivo PJ/PF**, adaptação **100% Mobile-First** e proteção da conversão dos canais digitais/OOH mesmo em propostas híbridas com Rádio.

---

## 👩‍💼 2. O Que Eu Fiz (Minha Atuação como PM)

* **Estruturação de Regras de Negócio Complexas (Multi-Veículo):** Desenhei a lógica financeira e de UX para separar canais de **liquidação imediata** (*OOH, Portais Globo e Revistas*) de canais com **faturamento pós-reserva de grade** (*Rádio CBN*), impedindo que a burocracia de um veículo travasse a venda dos demais.
* **Desenho de Jornada & Redução de Fricção (CRO):** Mapeei cada ponto de abandono no topo da proposta, nos cards de mídia e no checkout (Cartão em até 6x sem juros, PIX e Boleto), criando estados claros de ciclo de vida (*Aguardando pagamento*, *Campanha ativa* e *Campanha concluída com renovação em 1 clique*).
* **Liderança de UX Mobile-First & Arquitetura da Informação:** Defini a hierarquia de dados para o decisor PME que abre propostas pelo WhatsApp (comutação *Lista | Mapa*, eliminação de métricas redundantes nos *drawers*, rolagem inteligente no PIX mobile e reordenação hierárquica de faturamento).
* **Prototipação de Alta Fidelidade & Especificação Técnica:** Construí e validei o protótipo funcional navegável com dados reais e estados dinâmicos, acelerando o alinhamento com stakeholders e entregando a PRD pronta para engenharia com zero ambiguidade.

---

## 🎯 3. O Que Eu Resolvi (Dores Mapeadas)

1. **Paralisia de Decisão em Propostas Multicanal:** O cliente PME não entendia onde seus anúncios apareceriam fisicamente (OOH) nem a diferença entre métricas de *Impacto*, *Impressões* e *Inserções*.
2. **Bloqueio de Checkout por Regra Fiscal de Rádio:** O faturamento de Rádio exige confirmação prévia de disponibilidade na emissora; cobrar tudo junto travava o fechamento imediato de Telas OOH e Digital.
3. **Abandono no Cadastro de Faturamento:** Exigir dezenas de campos antes mesmo de o cliente explorar o plano de mídia gerava atrito precoce.
4. **Inviabilidade de Compartilhamento no WhatsApp:** Propostas exportadas em PDF com mapas e imagens chegavam a **~19 MB**, estourando limites de envio por e-mail corporativo e demorando para baixar no 4G.
5. **Experiência Mobile Quebrada no Pagamento:** Gerar QR Code de PIX na tela do próprio celular era inútil (o usuário não consegue escanear a própria tela com a câmera do mesmo aparelho).

---

## 🚧 4. Principais Desafios de Produto & Negócio

| Desafio | Como Resolvi (Decisão de Produto) |
| :--- | :--- |
| **Conciliar 4 canais com naturezas de mídia diferentes** | Padronizei as unidades de valor no cabeçalho de cada card (`impacto` em OOH, `impressões` em Digital/Revistas, `inserções` em Rádio) e limpei duplicidades nos *drawers* de detalhamento. |
| **Exibir dezenas de prédios e telas sem poluir a tela** | Criei o **agrupamento inteligente por condomínio** (consolidando Torres/Blocos em um único card com soma automática de telas) e sincronizei a lista com um **Mapa Interativo de 580px**. |
| **Cadastro PJ/PF sem quebrar o layout da proposta** | Implementei um **fluxo progressivo in-place** na Hero: primeiro o cliente escolhe PJ/PF e preenche apenas 4 dados essenciais; o endereço com busca automática por CEP (`ViaCEP`) abre sob demanda. |
| **Fazer o PDF executivo caber no WhatsApp (< 1 MB)** | Redesenhei o motor de exportação para renderizar páginas em JPEG otimizado + compressão de streams PDF, derrubando o arquivo de **18,77 MB para 309 KB** mantendo nitidez executiva. |
| **Ansiedade pós-geração de PIX ou Boleto** | Ao clicar em *"Ativar minha campanha"*, o botão principal muda imediatamente para estado inativo (`Aguardando pagamento`) e libera a confirmação ativa (`Já paguei o PIX` / `Já paguei o boleto`). |

---

## 📦 5. O Que Foi Entregue (Destaques da Solução)

* **Hero Contextual com Ciclo de Vida Completo:**
  * Suporte a 3 status de negócio: `Aguardando pagamento` (com timer de validade), `Campanha ativa` (com atalho para envio de criativos) e `Campanha concluída` (com CTA de **Renovação de Campanha**).
  * **Cadastro Progressivo de Faturamento (PJ e PF)** com máscaras automáticas e autopreenchimento de endereço via CEP.
* **Estimativa de Entrega Modular:**
  * Adaptação dinâmica do grid conforme o mix contratado: **Visão Multicanal** (1 card por canal) vs. **Visão Monocanal** (abertura em 4 KPIs profundos do canal único).
* **Aba 1 — Plano de Mídia Interativo:**
  * **Mapa Leaflet + Lista Sincronizada** para pontos OOH (Comerciais, Residenciais e Shoppings) no desktop e chaveador **Lista | Mapa** no mobile.
  * **Drawers/Popovers enxutos por canal:** remoção de métricas repetidas para leitura em 3 segundos.
* **Aba 2 — Checkout & Aprovação Inteligente:**
  * **Cartão de Crédito (1x a 6x sem juros)**, **PIX** e **Boleto Bancário** com paridade visual e funcional.
  * **Otimização Mobile-First no PIX:** ocultação de QR Code inútil no mobile, foco em *"Copiar código PIX"* e *smooth scroll* automático até o botão de ativação.
  * **Split Financeiro Automático:** isolamento do valor de **Rádio CBN** em card informativo de faturamento posterior (posicionado abaixo do checkout no mobile por hierarquia de conversão).
* **Exportações B2B Prontas para Decisores:**
  * **PDF Executivo Ultra-Leve (`0,30 MB`)** com métricas já na Página 1 e paginação adaptativa.
  * **Planilha Excel (`.xlsx`) Estilizada** com identidade visual Aqui Ads (`#F97316`), totais consolidados e autofiltros nativos.

---

## ⚖️ 6. Comparativo: Antes vs. Depois

| Dimensão | ❌ Antes (Abordagem Tradicional) | ✅ Depois (Nova Página de Propostas Aqui Ads) |
| :--- | :--- | :--- |
| **Apresentação do Plano** | PDF/Link estático sem visualização geográfica real das telas | **Mapa interativo sincronizado** + agrupamento inteligente de torres/condomínios |
| **Propostas com Rádio CBN** | Risco de travar todo o checkout esperando reserva manual da rádio | **Checkout Híbrido:** OOH + Digital pagos na hora; Rádio faturada após reserva |
| **Cadastro de Faturamento** | Formulário longo e intimidador logo na entrada | **Cadastro Progressivo (PJ/PF)** em 2 passos curtos com `ViaCEP` |
| **Leitura de Métricas no Mobile** | Rótulos genéricos ("impactos" para tudo) e informações duplicadas | **Taxonomia precisa por veículo** (`impacto`, `impressões`, `inserções`) sem redundância |
| **Pagamento PIX no Celular** | Exibição de QR Code (impossível de escanear no mesmo celular) | **Zero QR Code no mobile**, auto-scroll até ativação e cópia em 1 toque |
| **Pós-Clique no Checkout** | Botão continuava ativo, gerando cliques duplos e dúvida no cliente | Botão trava em **`Aguardando pagamento`** + opção clara de **`Já paguei`** (PIX/Boleto) |
| **Compartilhamento em PDF** | Arquivo pesado (**18,77 MB**), lento para baixar e enviar no WhatsApp | Arquivo ultra-leve (**0,30 MB / 309 KB** — **redução de 98,4%**) com layout executivo |
| **Pós-Campanha (Retenção)** | Proposta virava um link morto após o fim da veiculação | Estado **`Campanha concluída`** vira alavanca de **Renovação / Recompra** |

---

## 📈 7. Resultados & Impacto Gerado

* **-98,4% no tamanho do PDF comercial (`18,77 MB` $\rightarrow$ `0,30 MB`):** viabilizou o envio instantâneo pelo WhatsApp dos executivos comerciais e carregamento imediato no 4G dos clientes PME.
* **100% do Checkout OOH + Digital destravado:** separação arquitetural do faturamento de Rádio CBN protegeu o *cash collection* imediato no Cartão (até 6x), PIX e Boleto.
* **Redução drástica de carga cognitiva no Mobile:** eliminação de campos redundantes nos *drawers* de métricas, supressão do QR Code no celular e priorização visual do pagamento imediato sobre o faturamento futuro.
* **Time-to-Market acelerado entre Produto, Design e Engenharia:** entrega de protótipo 100% funcional + PRD completa com todos os estados de exceção mapeados.

---

## 🏁 8. Conclusão & Visão de Produto

Transformar uma **Página de Propostas B2B** em uma alavanca de receita exigiu olhar além da interface: foi necessário conectar **psicologia do comprador PME**, **regras operacionais de múltiplos veículos de mídia (OOH, Digital, Impresso e Rádio)** e **performance técnica de ponta (Mobile & PDF de 300 KB)**.

O resultado foi uma experiência que funciona tanto como **ferramenta de venda consultiva** para o time comercial quanto como **checkout self-service sem atrito** para o anunciante — do primeiro clique no WhatsApp até a renovação da campanha.

