# Death Acceptance

Procedimento de encerramento quando a hipótese falha.

---

## Quando executar

Após FASE 7 (Veredito), se a resposta for: **Hipótese foi refutada? Sim.**

---

## O que registrar

### 1. Congele o estado final

```bash
git tag -a "REFUTED" -m "Hypothesis failed on [data]"
git push origin REFUTED
```

Nenhum commit após refutação.

### 2. Documente a causa da morte

Crie `POST_MORTEM.md` com:

- Qual dado/teste matou a hipótese
- Em qual fase ocorreu
- Valor numérico da falha (se aplicável)
- Data do veredito

Não inclua:
- Justificativas
- Reinterpretações
- "Se tivéssemos feito X"
- "Talvez com mais tempo"

### 3. Liste o que aprendeu

Seção: **Lições extraídas**

- O que funcionou no processo
- O que não funcionou no processo  
- Suposições que estavam erradas

Não defenda a hipótese. Defenda o método.

---

## O que NÃO fazer

### Proibido:

- [ ] Ajustar parâmetros após veredito
- [ ] Reinterpretar o que "sucesso" significa
- [ ] Excluir dados que contradizem hipótese
- [ ] Introduzir hipóteses auxiliares não previstas
- [ ] Continuar trabalhando no modelo
- [ ] Renomear repositório para ocultar falha
- [ ] Deletar commits anteriores
- [ ] Argumentar que "não é refutação definitiva"

### Se você fizer qualquer item acima:

Você não está usando o protocolo.  
Você está blindando.

---

## Quando parar

Pare imediatamente após:

1. Registrar causa da morte
2. Criar tag REFUTED
3. Escrever POST_MORTEM.md
4. Fazer commit final

Não:
- Espere "ter certeza"
- Peça segunda opinião sobre o veredito
- Tente "uma última modificação"

O veredito foi dado na FASE 7.  
Esta fase só registra.

---

## Como seguir

### Separação necessária:

Hipótese ≠ Autor

A hipótese morreu.  
Você não.

Você testou.  
Você documentou.  
Você não blindou.

Isso é integridade.

### Próximo passo:

Se você tem outra hipótese:
- Crie novo repositório
- Comece na FASE 0
- Não carregue o modelo morto

Se não tem:
- Arquive este repositório
- Mantenha público
- Siga para outro projeto

---

## Sobre carregar o cadáver

Não transforme modelo refutado em:
- Identidade pessoal
- Batalha teórica
- Projeto de vida
- Vingança acadêmica

O modelo morreu. Deixe morto.

---

## Resultado nulo é resultado

Refutação documentada honestamente:
- Tem valor científico
- Evita que outros repitam erro
- Demonstra processo funcional
- Preserva integridade do autor

Você não falhou.

Você testou e aceitou o resultado.

Isso é ciência adulta.

---

## Checklist final

Antes de encerrar:

- [ ] Tag REFUTED criada?
- [ ] POST_MORTEM.md existe?
- [ ] Causa da morte documentada?
- [ ] Nenhuma justificativa inserida?
- [ ] Repositório congelado?
- [ ] Você separou hipótese de identidade?

Se todos "sim": processo completo.

---

## Aviso

Este arquivo não consola.

Ele encerra.
