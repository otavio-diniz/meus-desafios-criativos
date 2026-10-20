# Desafio Criativo — Planejando Automações com n8n Usando Apenas Bons Prompts

**Programa:** Santander 2026 — Automação com n8n (DIO)  
**Módulo:** 03 — Automatização de Processos com n8n  
**Tipo:** Material didático fictício/sintético de treino  
**Estado:** Prompt de planejamento produzido e revisado; **nenhum workflow implementado ou executado**  

## Problema e proposta

Materiais de estudo recebidos em uma pasta de entrada precisam ser identificados e classificados. Este desafio propõe **planejar**, por meio de um bom prompt, um workflow no n8n que consulte metadados de arquivos autorizados, sugira sua classificação acadêmica e produza um relatório para revisão humana.

O valor demonstrado está na clareza do objetivo, na sequência lógica de nodes e nas regras de segurança. Trata-se de **especificação didática**, não de uma integração com o Google Drive ou uma automação em produção.

## Prompt final — versão pública sanitizada

Atue como um especialista em n8n, automação de processos e organização de informações acadêmicas.
Quero planejar uma automação no n8n para identificar novos materiais acadêmicos recebidos na pasta "pasta de entrada de materiais acadêmicos autorizada", no Google Drive, e preparar sugestões de classificação por curso, módulo e pasta de destino.
Público ou responsável:
Pessoa responsável pela organização acadêmica, com revisão humana das classificações e decisões sobre o acervo.
Objetivo esperado:
Produzir um relatório de triagem contendo os novos arquivos identificados, sua possível classificação acadêmica, o destino recomendado, a justificativa e eventuais dúvidas ou divergências. As sugestões deverão passar por revisão humana antes de qualquer alteração no acervo.
Ferramentas envolvidas:
- n8n para orquestrar o workflow.
- Google Drive para consultar arquivos e referências autorizadas.
- Nodes como Manual Trigger, Google Drive, IF/Filter, Edit Fields e Merge, quando adequados.
- IA como recurso opcional para auxiliar na classificação.
- Relatório estruturado como saída do processo.
Etapas desejadas:
1. Iniciar o workflow por um gatilho manual. Considerar um Schedule Trigger apenas como possibilidade futura, sujeita a autorização.
2. Consultar os arquivos da pasta "pasta de entrada de materiais acadêmicos autorizada" em modo de leitura, coletando File ID, nome, tipo e metadados disponíveis.
3. Identificar arquivos novos e possíveis duplicidades.
4. Comparar os materiais com as referências acadêmicas autorizadas para sugerir curso, módulo e pasta de destino.
5. Aplicar filtros e condições para separar classificações consistentes, casos ambíguos e divergências.
6. Gerar um relatório com os dados de cada arquivo, classificação sugerida, justificativa, destino recomendado e status de validação.
7. Disponibilizar o relatório para análise e decisão humana.
Regras e restrições:
- Não mover, renomear, excluir nem modificar arquivos automaticamente.
- Não acessar documentos ou sistemas sem autorização.
- Não presumir que uma pasta foi integralmente examinada sem verificar seu conteúdo e eventuais subpastas ou atalhos.
- Não considerar nomes semelhantes como prova suficiente de duplicidade ou classificação.
- Preservar os File IDs e a proveniência dos arquivos.
- Marcar informações insuficientes, ambiguidades e divergências como "Pendente de validação".
- Não enviar dados sensíveis a serviços externos de IA sem autorização específica.
- Não converter presença de materiais em comprovação de aulas assistidas, atividades realizadas, notas ou conclusão de cursos.
- Não instalar ferramentas, configurar integrações reais ou executar o workflow nesta atividade.
O que você deverá entregar:
1. A sequência de nodes recomendados no n8n e a finalidade de cada um.
2. A descrição de como os dados passam entre as etapas.
3. As condições, validações e tratamentos de exceções necessários.
4. Um exemplo fictício de entrada e relatório de saída.
5. Os pontos em que a aprovação humana é obrigatória.
6. Possíveis melhorias futuras, claramente separadas do escopo inicial.
Apresente um plano claro, organizado e adequado a quem está aprendendo n8n. Não execute a automação nem assuma que integrações ou permissões já estão configuradas. Caso faltem informações essenciais, identifique-as explicitamente.

## Como avaliar este exercício

1. Leia o objetivo e confira se o processo, o público e o resultado desejado estão definidos.
2. Observe a sequência conceitual proposta: gatilho → consulta em modo de leitura → verificação de duplicidades → classificação sugerida → filtros/condições → relatório → revisão humana.
3. Verifique as salvaguardas: nenhum arquivo é movimentado automaticamente, ambiguidades são sinalizadas e progressos acadêmicos não são inferidos.
4. Distinga nodes **sugeridos para um desenho futuro** de funcionalidades já implementadas: este projeto entrega um prompt, não um arquivo JSON importável no n8n.

## Escopo, limitações e segurança

- **Não foi implementado nem executado um workflow**; não há testes de integração ou resultados operacionais.
- Não há acesso a pastas privadas, dados pessoais reais, credenciais, tokens ou mensagens enviadas neste artefato.
- A classificação é apenas uma sugestão: decisões materiais e modificações do acervo dependem de validação e autorização humanas.
- O campo de IA é opcional no plano conceitual; não há serviço externo de IA acionado.
- Dados sintéticos ou exemplos hipotéticos não constituem comprovação institucional.
- A **publicação no GitHub não comprova submissão, avaliação, nota, aprovação ou certificado da DIO**.

## Autoria e proveniência

Material autoral de treino de **Otávio Diniz**, desenvolvido com apoio de IA e revisado pelo autor. Inspirado no enunciado do desafio criativo do programa educacional Santander 2026 / DIO. O texto reproduz apenas a solução de planejamento criada para o exercício; **não inclui capturas, transcrições ou materiais didáticos de terceiros**.

As marcas e os nomes de plataformas mencionados pertencem a seus respectivos titulares. Não há afiliação ou endosso institucional implícito. Consulte [LICENSE](../../../LICENSE) e [NOTICE.md](../../../NOTICE.md) para condições de direitos e proveniência.
