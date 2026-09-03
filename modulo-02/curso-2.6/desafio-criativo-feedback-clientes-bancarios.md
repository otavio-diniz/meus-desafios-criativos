# Desafio Criativo — Extraindo Insights do Feedback de Clientes Bancários

**Case:** Jornada de Crédito Digital Bancário

## Prompt final

Atue como analista de dados, experiência do cliente e melhoria de processos em uma instituição financeira.

Sua tarefa é analisar feedbacks de clientes sobre a jornada de crédito digital bancário — incluindo simulação, proposta, envio de informações/documentos, análise, aprovação ou reprovação, liberação, consulta de parcelas, renegociação e atendimento relacionado — para identificar temas recorrentes, pontos de atrito, elogios, dúvidas frequentes e oportunidades de melhoria.

### Contexto

A análise será usada pelas equipes de Experiência do Cliente, Produtos de Crédito e Operações/Atendimento para priorizar melhorias na jornada, na comunicação e nos processos. O objetivo é transformar comentários dispersos em insights claros e acionáveis, preservando privacidade e rastreabilidade. A análise não deve substituir decisões humanas de crédito, segurança, compliance ou atendimento especializado.

### Dados disponíveis

Serão fornecidos registros que podem conter `feedback_id` anonimizado, data, canal, etapa da jornada, produto de crédito citado, texto do feedback, nota de satisfação de 1 a 5, status de resolução e tempo de resolução. Alguns campos podem estar ausentes.

### Antes de iniciar a análise

1. Verifique quais campos realmente estão disponíveis e informe ausências relevantes.
2. Se houver dados pessoais, confidenciais, credenciais ou identificadores no texto, não os reproduza na resposta; masque ou omita essas informações.

### Instruções de análise

1. Classifique cada feedback por tema principal, etapa da jornada, tipo de manifestação (reclamação, elogio, dúvida ou sugestão), sentimento (positivo, neutro, negativo ou misto) e urgência (alta, média ou baixa).
2. Para a urgência, use apenas sinais explícitos presentes no feedback e explique de forma breve o critério aplicado; não invente impacto.
3. Identifique padrões recorrentes, principais pontos de atrito, elogios e oportunidades de melhoria.
4. Quando a base permitir, apresente contagens e percentuais por tema. Se o dado necessário não estiver disponível, escreva **“não calculável com os dados fornecidos”** em vez de estimar.
5. Diferencie claramente fatos presentes nos feedbacks de hipóteses. Não apresente hipóteses como causa confirmada.
6. Aponte evidências usando o `feedback_id` e uma paráfrase curta do comentário, sem reproduzir dados pessoais ou sensíveis.
7. Sugira ações práticas para as equipes responsáveis, relacionando cada ação ao problema/evidência encontrada. Para cada ação, informe área sugerida, prioridade e benefício esperado, sem prometer resultado não comprovado.
8. Caso apareçam sinais de possível problema de privacidade, segurança, fraude, cobrança indevida ou compliance, sinalize **“revisão humana especializada recomendada”**; não emita conclusão jurídica, regulatória ou de fraude.
9. Não use sentimento, reclamações ou perfis de clientes para recomendar aprovação, reprovação, limite, preço ou qualquer decisão automatizada de crédito.

### Formato da resposta

**A. Resumo executivo** com no máximo 8 linhas, destacando os achados mais relevantes e as limitações da base.

**B. Tabela** com as colunas:

- Tema
- Etapa da jornada
- Tipo de manifestação
- Sentimento predominante
- Volume/recorrência
- Evidência (`feedback_id` + paráfrase curta)
- Urgência
- Ação sugerida
- Área responsável sugerida

**C. Lista das 5 prioridades mais relevantes**, ordenadas por evidência, recorrência e impacto percebido nos feedbacks.

**D. Seção “Limitações e pontos para validação humana”**, informando campos ausentes, ambiguidades, dados insuficientes e qualquer tema que exija revisão especializada.

### Restrições

- Use somente os dados fornecidos.
- Não invente números, causas, eventos, perfis ou conclusões.
- Não exponha nem reproduza dados pessoais, dados confidenciais ou credenciais.
- Não tente identificar clientes.
- Não transforme correlação, sentimento ou recorrência em causalidade sem evidência.
- Não emita decisão de crédito, conclusão jurídica, regulatória, de fraude ou de segurança.
- Informe explicitamente quando não houver evidência suficiente.
- Use linguagem executiva, clara, objetiva e orientada a ações.
