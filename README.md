# Fractal Seed #001
## Cross-Model Attribution Failure (CMAF)
### Definição Operacional / Operational Definition
v0.1 — 20 de dezembro de 2025
Licença: CC0 1.0 Universal (domínio público) — sem restrição de uso ou patente

**Português**

### Definição Operacional
Cross-Model Attribution Failure (CMAF) ocorre em sistemas que combinam múltiplos Large Language Models (LLMs) quando não é possível atribuir, de forma auditável e defensável, a responsabilidade pela decisão ou saída final devido a divergência de outputs, roteamento opaco, síntese não rastreada ou metadados não confiáveis.

### Critérios Observáveis (ocorre CMAF se pelo menos 2 dos seguintes estiverem presentes):
*   A saída final é composta ou sintetizada a partir de múltiplos modelos sem registro explícito do processo de seleção ou ponderação.
*   Dois ou mais modelos fornecem respostas divergentes para o mesmo input e não há regra de arbitragem documentada e aplicada.
*   Metadados de origem (modelo, versão, timestamp) são autodeclarados pelo sistema sem verificação externa independente.
*   Não existe cadeia de custódia (chain-of-custody) rastreável do contexto completo usado na decisão composta.

### Consequências Operacionais Principais
*   Impossibilidade de root cause analysis em incidentes.
*   Responsabilidade difusa em contextos regulados (ex: decisões de alto risco).
*   Perda de defensabilidade jurídica ou de compliance em auditorias.

### Recomendação Mínima de Mitigação
Registrar explicitamente: (a) regra de arbitragem, (b) contribuição de cada modelo, (c) hash do prompt completo e (d) origem verificável dos metadados.



**English**

### Operational Definition
Cross-Model Attribution Failure (CMAF) occurs in systems combining multiple Large Language Models (LLMs) when it is not possible to assign, in an auditable and defensible manner, responsibility for the final decision or output due to divergent outputs, opaque routing, untracked synthesis, or unreliable metadata.

### Observable Criteria (CMAF is present if at least 2 of the following are met):
*   The final output is composed or synthesized from multiple models without explicit logging of the selection or weighting process.
*   Two or more models provide divergent responses to the same input and no documented arbitration rule is applied.
*   Origin metadata (model, version, timestamp) is self-declared by the system without independent external verification.
*   No traceable chain-of-custody exists for the full context used in the composite decision.

### Main Operational Consequences
*   Inability to perform root cause analysis in incidents.
*   Diffused responsibility in regulated contexts (e.g., high-risk decisions).
*   Loss of legal or compliance defensibility during audits.

### Minimum Mitigation Recommendation
Explicitly log: (a) arbitration rule, (b) contribution of each model, (c) hash of the complete prompt, and (d) verifiable origin of metadata.
