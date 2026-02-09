# Protocol

Nove fases obrigatórias para testar hipóteses descartáveis.

## FASE 0: Condição inicial

**Objetivo**: Definir estado zero.

**Ações**:
1. Identifique a hipótese em uma frase
2. Pergunte: "Qual dado pode matar isso?"
3. Se não souber responder → PARAR
4. Documente a resposta

**Saída**: Hipótese nomeada + dado mortal identificado.

---

## FASE 1: Modelo mínimo

**Objetivo**: Formalizar hipótese em linguagem testeável.

**Ações**:
1. Escreva equações/algoritmo/regras
2. Liste parâmetros livres
3. Defina que observável testa
4. Documente suposições explícitas

**Saída**: Modelo formalizado em MODEL.md

**Critério de aceitação**: Outra pessoa pode implementar sem perguntar.

---

## FASE 2: Dados reais

**Objetivo**: Obter dados observacionais ou experimentais.

**Ações**:
1. Identifique fontes de dados públicas
2. Liste limitações dos dados
3. Documente incertezas
4. Organize em formato padrão (CSV/JSON)

**Saída**: Dados em data/ + documentação em DATA.md

**Restrição**: Não use dados sintéticos para teste final.

---

## FASE 3: Implementação

**Objetivo**: Codificar modelo.

**Ações**:
1. Implemente modelo em código
2. Adicione testes unitários
3. Verifique casos limite
4. Documente dependências

**Saída**: Código em src/ + requirements.txt

**Critério**: Código roda sem erro em ambiente limpo.

---

## FASE 4: Teste estatístico

**Objetivo**: Confrontar modelo com dados.

**Ações**:
1. Calcule métrica de ajuste (χ², likelihood, etc.)
2. Compare com modelo nulo/baseline
3. Documente resultado numérico
4. NÃO interprete ainda

**Saída**: Resultado bruto em RESULT_RAW.md

---

## FASE 5: Comparação honesta

**Objetivo**: Verificar se modelo sobrevive.

**Ações**:
1. Compare com modelos padrão da área
2. Liste onde seu modelo é pior
3. Liste onde é melhor
4. Não omita o que falhou

**Saída**: Comparação em COMPARISON.md

**Regra**: Citar fontes dos modelos baseline.

---

## FASE 6: Análise de sensibilidade

**Objetivo**: Testar robustez.

**Ações**:
1. Varie parâmetros livres
2. Teste com diferentes subconjuntos de dados
3. Verifique se conclusão muda
4. Documente quando modelo colapsa

**Saída**: SENSITIVITY.md

---

## FASE 7: Veredito explícito

**Objetivo**: Decidir: sobreviveu ou morreu?

**Ações**:
1. Responda: Hipótese foi refutada? (Sim/Não)
2. Justifique com dados da Fase 4-6
3. Se sobreviveu: liste o que ainda pode matá-la
4. Se morreu: documente causa da morte

**Saída**: VERDICT.md

**Regra**: Sem ambiguidade. "Parcialmente" não é resposta.

---

## FASE 8: Pós-veredito

**Objetivo**: Preparar para uso ou descarte.

### Se sobreviveu:
1. Liste próximos testes necessários
2. Identifique limitações conhecidas
3. Prepare para publicação/compartilhamento

### Se morreu:
1. Documente lições aprendidas
2. Arquive sem apagar
3. Não tente ressuscitar com ajustes ad-hoc

**Saída**: POST_MORTEM.md ou NEXT_STEPS.md

---

## Regras gerais

1. **Não pule fases**  
   Cada fase depende da anterior.

2. **Documente antes de interpretar**  
   Dados primeiro, narrativa depois.

3. **CHECKLIST.md antes de cada fase**  
   Verifique condições de entrada.

4. **Se em dúvida, PARAR**  
   Clareza precede execução.

5. **Refutação é resultado**  
   Não é fracasso.

---

## Vocabulário preciso

Ver `VOCABULARY.md` para definições operacionais de:
- Hipótese descartável
- Dado mortal
- Blindagem
- Refutação honesta
