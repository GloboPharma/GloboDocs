# 📊 MATRIZ DE GAP ANALYSIS  
## Governança Documental TI – Ambiente Regulado (ANVISA / GxP / ISO 27001)

### Referências Regulatórias

- ANVISA  
- ISO/IEC 27001  
- RDC 301/2019  

---

# 1️⃣ Política Formal de Governança
## Objetivo
Avaliar a existência, formalização e aprovação da política de governança documental aplicável à área de TI em ambiente regulado.

## Análise de Lacunas

| Requisito | Situação Atual | Gap Identificado | Risco | Ação Recomendada | Prioridade |
|------------|---------------|------------------|--------|------------------|------------|
| Política formal aprovada | Parcial / Inexistente | Ausência de aprovação formal | Não conformidade regulatória | Formalizar documento + assinatura digital ou aprovação via PR | Alta |
| Definição de papéis (Autor/Revisor/Aprovador) | Parcial | Falta evidência formal | Fragilidade de rastreabilidade | Criar matriz RACI oficial | Média |
| Classificação documental | Inexistente | Sem categorização | Exposição indevida de informação | Implementar classificação (Interno/Confidencial/GxP) | Alta |

---

# 2️⃣ Controle de Mudanças

## Objetivo
Avaliar se as alterações documentais seguem fluxo controlado, versionado e aprovado formalmente.

## Análise de Lacunas

| Requisito | Situação Atual | Gap Identificado | Risco | Ação Recomendada | Prioridade |
|------------|---------------|------------------|--------|------------------|------------|
| Registro formal de mudança | Manual / inexistente | Falta padronização | Falha crítica em auditoria | Implementar template obrigatório | Alta |
| Avaliação de Impacto GxP | Inexistente | Sem análise regulatória | Risco regulatório direto | Criar formulário padrão de Impact Assessment | Alta |
| Histórico de versões | Git simples | Sem controle de aprovação | Falta evidência formal | Bloquear merge direto na main | Alta |

---

# 3️⃣ Integridade e Controle Técnico

## Objetivo
Garantir proteção contra alterações não autorizadas e assegurar rastreabilidade técnica.

## Análise de Lacunas

| Requisito | Situação Atual | Gap Identificado | Risco | Ação Recomendada | Prioridade |
|------------|---------------|------------------|--------|------------------|------------|
| Branch protegida | Não verificado | Pode não estar ativa | Alterações não autorizadas | Ativar proteção de branch | Alta |
| PR obrigatório | Não verificado | Pode não existir | Falha de segregação | Exigir aprovação mínima | Alta |
| Logs auditáveis | Git possui | Não formalizado | Falta evidência documentada | Criar procedimento de evidência | Média |
| Backup do repositório | Desconhecido | Possível falha | Perda de documentação | Ativar backup automatizado | Alta |

---

# 4️⃣ Classificação GxP de Sistemas

## Objetivo
Verificar se os sistemas estão inventariados, classificados e vinculados à documentação correspondente.

## Análise de Lacunas

| Requisito | Situação Atual | Gap Identificado | Risco | Ação Recomendada | Prioridade |
|------------|---------------|------------------|--------|------------------|------------|
| Inventário de sistemas | Parcial | Não centralizado | Falta de rastreabilidade | Criar catálogo oficial | Alta |
| Classificação GxP | Inexistente | Sem avaliação formal | Não conformidade grave | Implementar matriz de impacto GxP | Alta |
| Vinculação documento ↔ sistema | Não estruturado | Desconexão documental | Falha em auditoria | Criar campo obrigatório nos templates | Média |

---

# 5️⃣ Publicação e Status

## Objetivo
Garantir controle de ciclo de vida dos documentos e evitar uso de versões incorretas.

## Análise de Lacunas

| Requisito | Situação Atual | Gap Identificado | Risco | Ação Recomendada | Prioridade |
|------------|---------------|------------------|--------|------------------|------------|
| Status do documento (Vigente/Obsoleto) | Inexistente | Sem controle de ciclo de vida | Uso de versão incorreta | Implementar campo obrigatório | Alta |
| Arquivamento controlado | Não formalizado | Risco de uso indevido | Não conformidade | Criar pasta /archive | Média |

---

# Conclusão Geral

A maturidade atual depende da implementação formal de:

- Política aprovada
- Controle estruturado de mudanças
- Classificação GxP
- Proteção técnica do repositório
- Controle de ciclo de vida documental

A priorização deve focar inicialmente em riscos regulatórios (Alta prioridade).
