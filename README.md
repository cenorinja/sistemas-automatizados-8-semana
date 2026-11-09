# Semana 8 — Sistemas Supervisórios

## Entrega
- `tags.csv`: dicionário de tags do protótipo.
- `casos_teste.csv`: casos de teste com resultado esperado, campos para resultado obtido e situação.
- `capturas/`: local destinado às capturas reais.
- `roteiro_inspecao.pdf`: ficha de revisão por pares e evidências necessárias.

## Link do protótipo Figma
INSERIR AQUI O LINK REAL DE VISUALIZAÇÃO DO FIGMA (modo Present/visualização).
O link deve ser testado em janela anônima ou por outra pessoa, sem depender da conta do autor.

## Escopo do protótipo
Supervisório didático para reservatório e bomba P-101, com estados GOOD, H e HH, tendência histórica do nível, qualidade de comunicação e matriz de permissivos.

Parâmetros de exemplo adotados nesta documentação:
- Nível normal de teste: 58%.
- Limite H: 70%.
- Limite HH: 90%.
- Caso de atenção: 78%.
- Caso de alarme alto-alto: 92%.

Os limites são parâmetros propostos para o exercício e devem ser ajustados se o projeto original tiver outros valores.

## Revisão por pares — roteiro de inspeção
1. Localizar nível e modo de operação em até cinco segundos.
2. Encontrar o alarme mais crítico e identificar sua descrição.
3. Tentar um comando remoto não permitido em ambiente de protótipo/simulação; confirmar que o sistema bloqueia e explica o motivo.
4. Retornar à visão geral em um passo.
5. Registrar três melhorias com justificativa.

## Três melhorias justificadas sugeridas
1. **Hierarquia visual do nível e do modo:** manter nível, unidade e modo na área superior da tela, reduzindo o tempo de procura.
2. **Alarme HH com texto, prioridade e registro:** não depender somente da cor; apresentar descrição, horário e reconhecimento.
3. **Bloqueio com motivo explícito:** quando comunicação estiver BAD ou o modo for LOCAL, desabilitar o comando remoto e informar a primeira causa impeditiva.

## Evidências a anexar
Substitua os nomes de exemplo na pasta `capturas/` por capturas reais:
- T01 normal (58% / GOOD)
- T02 atenção (78% / H)
- T03 alarme HH (92%)
- T04 comunicação ruim (COMM_PLC-BAD)
- T05 confirmação de parada P-101
- T06 tentativa de comando remoto em modo local
- T07 retorno à visão geral
- T08 indicação de qualidade BAD/UNCERTAIN

## Integridade das evidências
Os arquivos CSV e o roteiro são modelos preparados para a atividade. Eles não são capturas de execução. Preencha `resultado_obtido` e `situacao` somente depois de testar o protótipo. Não declare aprovação sem evidência observável.
