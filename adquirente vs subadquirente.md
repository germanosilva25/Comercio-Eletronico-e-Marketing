Adquirente e subadquirente são dois termos importantes no sistema de pagamentos eletrônicos, especialmente quando se trata de transações com cartões de crédito e débito. Ambos desempenham papéis distintos, mas complementares, no processamento de pagamentos. Vamos explorar cada um em detalhes.

### 1. **Adquirente (Acquirer)**

**O que é?**
Um adquirente, também conhecido como "banco adquirente" ou "acquirer," é uma instituição financeira licenciada para processar transações de cartões de crédito e débito em nome dos comerciantes. Em termos simples, o adquirente é o intermediário entre o comerciante (ou loja) e a rede de cartões (como Visa, Mastercard, etc.).

**Funções do Adquirente:**
- **Processamento de Pagamentos:** O adquirente processa as transações feitas por cartões de crédito e débito. Ele se conecta à rede de cartões para autorizar e capturar as transações.
- **Relacionamento com Redes de Cartões:** O adquirente possui um contrato com as redes de cartões, permitindo que os comerciantes aceitem esses cartões como método de pagamento.
- **Liquidação:** Após a autorização da transação, o adquirente facilita a transferência dos fundos do banco emissor do cartão para a conta do comerciante.
- **Gestão de Risco e Fraude:** O adquirente monitora as transações para detectar atividades fraudulentas e minimizar os riscos.
- **Conformidade Regulamentar:** O adquirente é responsável por garantir que todas as transações estejam em conformidade com as regulamentações do setor de pagamentos (como o PCI DSS).

**Exemplos de Adquirentes:**
- Cielo
- Rede
- Getnet
- Stone

### 2. **Subadquirente (Subacquirer)**

**O que é?**
Um subadquirente, também conhecido como "facilitador de pagamento" ou "payment facilitator," é uma empresa que oferece serviços de pagamento para comerciantes, mas sem a necessidade de se tornarem adquirentes completos. Os subadquirentes atuam como intermediários entre os comerciantes e os adquirentes, permitindo que pequenos negócios ou empreendedores aceitem pagamentos sem a necessidade de ter uma conta direta com um adquirente.

**Funções do Subadquirente:**
- **Intermediação:** O subadquirente faz a ponte entre os comerciantes e os adquirentes, agrupando várias contas de comerciantes sob uma única conta de adquirente.
- **Onboarding Simplificado:** O subadquirente facilita o processo de adesão para os comerciantes, oferecendo uma integração simplificada e sem a necessidade de complexos processos de aprovação.
- **Serviços Complementares:** Além de processar pagamentos, os subadquirentes frequentemente oferecem serviços adicionais, como emissão de boletos, gestão de risco, antifraude, e relatórios de transações.
- **Distribuição de Fundos:** Os subadquirentes recebem os fundos das transações e os distribuem para as contas dos comerciantes individuais, geralmente após deduzirem as taxas de serviço.
- **Gestão da Experiência do Usuário:** O subadquirente geralmente fornece a interface de pagamento e suporte ao cliente, atuando como o ponto de contato principal para o comerciante.

**Exemplos de Subadquirentes:**
- PayPal
- PagSeguro
- Mercado Pago
- Stripe

### 3. **Diferenças Entre Adquirente e Subadquirente:**

| **Aspecto**                     | **Adquirente**                                      | **Subadquirente**                                   |
|---------------------------------|----------------------------------------------------|----------------------------------------------------|
| **Definição**                   | Instituição financeira que processa pagamentos diretamente para os comerciantes. | Intermediário que agrupa comerciantes e facilita pagamentos via adquirente. |
| **Relação com o Comerciante**   | Relacionamento direto, requer contrato específico e análise de risco para cada comerciante. | Relacionamento indireto, com integração rápida e simplificada para o comerciante. |
| **Processo de Onboarding**      | Processo mais rigoroso e demorado, envolvendo análise de crédito e conformidade. | Processo mais rápido e simplificado, com menos burocracia. |
| **Gestão de Risco**             | O adquirente tem controle direto sobre a gestão de risco e fraude. | O subadquirente gerencia o risco para seus comerciantes, mas o adquirente ainda pode impor requisitos. |
| **Controle e Flexibilidade**    | Mais controle sobre as transações e relação direta com redes de cartões. | Menos controle, pois depende das políticas do subadquirente. |
| **Conformidade Regulamentar**   | Altamente regulado, deve estar em conformidade com as normas do setor (como PCI DSS). | Também deve estar em conformidade, mas muitas responsabilidades são delegadas ao adquirente. |
| **Exemplos**                    | Cielo, Rede, Getnet, Stone                          | PayPal, PagSeguro, Mercado Pago, Stripe            |

### 4. **Detalhes do Adquirente:**

- **Infraestrutura e Licenciamento:** Adquirentes são instituições licenciadas para operar como membros da rede de cartões, como Visa ou Mastercard. Eles têm a infraestrutura necessária para lidar com grandes volumes de transações.
  
- **Modelos de Tarifas:** Os adquirentes normalmente cobram taxas por transação, que podem incluir uma taxa fixa por transação e um percentual sobre o valor da transação. Essas tarifas cobrem os custos de processamento e gerenciamento de riscos.

- **Segurança:** Como parte da sua função, os adquirentes investem fortemente em segurança e conformidade para proteger os dados das transações e minimizar fraudes.

- **Liquidação de Fundos:** O adquirente é responsável por garantir que os fundos das transações sejam liquidados e transferidos para a conta do comerciante em prazos que variam de acordo com o contrato.

### 5. **Detalhes do Subadquirente:**

- **Simplificação do Processo:** Os subadquirentes tornam mais fácil para pequenos comerciantes, freelancers ou startups aceitarem pagamentos eletrônicos sem a necessidade de estabelecer uma conta direta com um adquirente.

- **Flexibilidade de Serviços:** Subadquirentes frequentemente oferecem uma gama mais ampla de serviços além do simples processamento de pagamentos, como soluções de e-commerce, APIs de pagamento, e integrações com sistemas de contabilidade.

- **Gestão de Conta Unificada:** Em vez de cada comerciante ter uma conta separada com o adquirente, o subadquirente gerencia uma conta principal e distribui os fundos aos comerciantes.

- **Controle de Taxas:** O subadquirente tem a flexibilidade de definir suas próprias taxas e condições de serviço, que podem ser diferentes das praticadas diretamente pelos adquirentes.

---

### 6. **Tabela Comparativa:**

| **Critério**                     | **Adquirente**                                      | **Subadquirente**                                   |
|----------------------------------|----------------------------------------------------|----------------------------------------------------|
| **Licenciamento e Regulamentação** | Licenciado como membro direto de redes de cartões e altamente regulado. | Não requer licenciamento direto de redes de cartões; opera sob licenças de adquirentes. |
| **Relacionamento com Redes de Cartões** | Direto, com contrato formal e responsabilidade total. | Indireto, via adquirente, sem relação direta com as redes de cartões. |
| **Simplicidade para o Comerciante** | Processo de adesão mais complexo, ideal para empresas maiores. | Processo simplificado, ideal para pequenas empresas e empreendedores. |
| **Responsabilidade por Conformidade** | Total responsabilidade pelas conformidades (PCI DSS, etc.). | Responsável pela conformidade, mas algumas responsabilidades são compartilhadas com o adquirente. |
| **Gestão de Fraude e Risco**     | Controle total sobre ferramentas e políticas de gestão de fraude. | Gestão de risco e fraude, mas com dependência das políticas do adquirente. |
| **Serviços Oferecidos**          | Principalmente processamento de pagamentos.         | Processamento de pagamentos e serviços adicionais (e-commerce, boletos, etc.). |
| **Exemplos de Empresas**         | Cielo, Rede, Getnet, Stone                          | PayPal, PagSeguro, Mercado Pago, Stripe            |

---

Em resumo, adquirentes e subadquirentes desempenham papéis essenciais no processamento de pagamentos, mas com níveis diferentes de responsabilidade, complexidade e serviços oferecidos. Os adquirentes são mais adequados para grandes empresas que precisam de controle total sobre suas transações, enquanto os subadquirentes oferecem uma solução mais acessível e flexível para pequenas empresas e empreendedores.