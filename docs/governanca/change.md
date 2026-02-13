# Gestão de Mudanças (Change Management)

O objetivo da **Gestão de Mudanças** na Globo Pharma é garantir que métodos e procedimentos padronizados sejam utilizados para o tratamento eficiente e rápido de todas as alterações na infraestrutura, sistemas ou processos, minimizando o impacto de incidentes relacionados a mudanças no atendimento aos clientes e na operação.

## 🎯 Objetivos do Processo

* **Minimizar Riscos:** Avaliar o impacto de cada mudança antes de sua execução.
* **Transparência:** Garantir que todas as áreas afetadas sejam comunicadas.
* **Rastreabilidade:** Manter um histórico auditável de quem, quando e por que algo foi alterado.
* **Sucesso na Execução:** Reduzir o número de mudanças que precisam ser revertidas (*rollback*).

---

## 🚦 Tipos de Mudança

No portal **GloboDocs**, classificamos as mudanças em três categorias:

1.  **Mudança Padrão:** Mudanças de baixo risco, pré-autorizadas e que seguem um procedimento estabelecido (ex: atualização de antivírus).
2.  **Mudança Normal:** Segue o fluxo completo de avaliação, planejamento e aprovação pelo comitê responsável.
3.  **Mudança de Emergência:** Implementada o mais rápido possível para resolver um incidente crítico ou evitar uma interrupção grave.

---

## 🛠️ Fluxo de Aprovação

Para que uma mudança seja implementada, ela deve seguir as etapas abaixo:

### 1. Registro da Requisição de Mudança (RFC)
Toda mudança deve ser documentada contendo:
* Descrição da alteração.
* Justificativa (motivo da mudança).
* Plano de Implementação.
* **Plano de Contingência (Rollback):** Como voltar ao estado anterior se algo falhar.

### 2. Avaliação e Aprovação
Dependendo da criticidade, a mudança deve ser aprovada pelo **Comitê de Controle de Mudanças (CAB)**.

**"Papéis e Responsabilidades"**
    A aprovação de mudanças estratégicas segue a **Matriz RACI** definida na seção de [Governança: Matriz RACI](raci.md).

---

## 📝 Ciclo de Vida da Mudança

| Fase | Descrição | Responsável |
| :--- | :--- | :---: |
| **Planejamento** | Definição técnica e análise de impacto. | **R** |
| **Aprovação** | Validação da gerência ou comitê. | **A** |
| **Execução** | Implementação técnica da alteração. | **R** |
| **Pós-Implementação** | Verificação de sucesso e encerramento. | **R/A** |

---

## ⚠️ Plano de Rollback

É obrigatório que toda mudança "Normal" ou "Emergencial" possua um plano de reversão testado. Caso a janela de execução ultrapasse o tempo previsto ou ocorram erros críticos, a mudança deve ser interrompida e o sistema restaurado.

---
_Última atualização: 2026_
