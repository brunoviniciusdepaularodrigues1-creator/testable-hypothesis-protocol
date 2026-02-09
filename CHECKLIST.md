# Checklist

Verificação sim/não antes de cada fase.

Se qualquer resposta for "não" → a fase não passou.

---

## FASE 0: Condição inicial

- [ ] A hipótese está escrita em uma frase?
- [ ] Existe ao menos um dado que pode refutá-la?
- [ ] Você consegue nomear esse dado agora?
- [ ] O dado é observável/mensurável?
- [ ] Você aceita parar se não souber responder?

---

## FASE 1: Modelo mínimo

- [ ] O modelo está formalizado (equações/algoritmo/regras)?
- [ ] Todos os parâmetros livres estão listados?
- [ ] Está claro qual observável o modelo testa?
- [ ] As suposições estão documentadas?
- [ ] Outra pessoa pode implementar sem perguntar?
- [ ] O modelo pode falhar?

---

## FASE 2: Dados reais

- [ ] Os dados são reais (não sintéticos)?
- [ ] A fonte dos dados está documentada?
- [ ] As incertezas estão quantificadas?
- [ ] As limitações dos dados estão listadas?
- [ ] Os dados estão organizados em formato padrão?
- [ ] Você pode reproduzir a obtenção dos dados?

---

## FASE 3: Implementação

- [ ] O código roda sem erro em ambiente limpo?
- [ ] Existem testes unitários?
- [ ] Os casos limite foram verificados?
- [ ] As dependências estão documentadas?
- [ ] O código reproduz o modelo da FASE 1?
- [ ] Você testou com dados de validação?

---

## FASE 4: Teste estatístico

- [ ] A métrica de ajuste foi calculada?
- [ ] Existe comparação com modelo nulo/baseline?
- [ ] O resultado está documentado numericamente?
- [ ] Você evitou interpretar antes de documentar?
- [ ] As incertezas estatísticas estão calculadas?
- [ ] O resultado pode refutar a hipótese?

---

## FASE 5: Comparação honesta

- [ ] O modelo foi comparado com padrões da área?
- [ ] Está documentado onde o modelo é pior?
- [ ] Está documentado onde o modelo é melhor?
- [ ] Nada foi omitido?
- [ ] As fontes dos modelos baseline estão citadas?
- [ ] A comparação é quantitativa?

---

## FASE 6: Análise de sensibilidade

- [ ] Os parâmetros livres foram variados?
- [ ] Diferentes subconjuntos de dados foram testados?
- [ ] Está documentado quando o modelo colapsa?
- [ ] A conclusão muda com variações ra- [ ] A robustez está quantificada?
- [ ] Os limites de validade estão claros?

---

## FASE 7: Veredito explícito

- [ ] A pergunta "Hipótese foi refutada?" tem resposta sim/não?
- [ ] A justificativa usa dados das fases 4-6?
- [ ] Se sobreviveu: está listado o que ainda pode matá-la?
- [ ] Se morreu: a causa da morte está documentada?
- [ ] Não há ambiguidade?
- [ ] Você evitou "parcialmente"?

---

## FASE 8: Pós-veredito

### Se sobreviveu:
- [ ] Os próximos testes estão listados?
- [ ] As limitações conhecidas estão documentadas?
- [ ] O trabalho está pronto para compartilhamento?

### Se morreu:
- [ ] As lições aprendidas estão documentadas?
- [ ] O trabalho foi arquivado (não apagado)?
- [ ] Você evitou ajustes ad-hoc para ressuscitar?
- [ ] A morte foi aceita sem reinterpretação?

---

## Verificação contínua

- [ ] Nenhuma fase foi pulada?
- [ ] Documentação precede interpretação?
- [ ] Clareza precede execução?
- [ ] Refutação é tratada como resultado, não fracasso?
- [ ] O autor está separado da hipótese?
