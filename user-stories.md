# 📖 HISTORIA-USUARIO.md

```markdown
# 📋 História de Usuário - TaskFlow

## 🎭 Cenário: Seu Primeiro Dia Como Dev Júnior

---

### 🏢 Bem-vindo à TaskFlow Inc.!

Parabéns! Você acabou de ser **contratado** como **Desenvolvedor Front-End Júnior** pela empresa **TaskFlow Inc.**

Hoje é seu primeiro dia de trabalho. Você acabou de chegar no escritório, pegou seu café, ligou seu computador e recebeu seu primeiro e-mail de trabalho...

---

## 📧 Email Recebido

De: Maria Silva <maria.silva@taskflow.com>
Para: Você <voce@taskflow.com>
Assunto: 🚀 Seu primeiro projeto - Sistema de Tarefas para Vendas
Data: Segunda-feira, 07 de Abril de 2025 - 09:00

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Olá!

Seja muito bem-vindo(a) à equipe TaskFlow! 🎉

Como conversamos na entrevista, você vai começar com um projeto real
e importante para a empresa. Deixa eu te contextualizar:

Nossa equipe de vendas está crescendo muito rápido. Hoje somos 15 vendedores
e o problema é: estamos PERDIDOS com nossas tarefas diárias.

Tentamos usar apps prontos, mas são muito complexos ou não têm as funções
que precisamos. Tentamos papel, mas... bom, você já sabe como acaba 😅

Então decidimos: vamos criar nosso próprio sistema! Simples, direto ao ponto,
do jeito que precisamos.

E é aí que você entra! 🚀

Seu desafio: criar um aplicativo web de To-Do List (lista de tarefas) que
atenda nossas necessidades.

Anexei os requisitos detalhados que levantei com a equipe.
O prazo é até próxima segunda (14/04).

Qualquer dúvida, pode me chamar! Estou aqui para ajudar.

Boa sorte no seu primeiro projeto! Confiamos em você! 💪

Abraços,
Maria Silva
Gerente de Vendas
TaskFlow Inc.

━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

---

## 📎 Anexo: Requisitos do Cliente

### 📋 Documento de Requisitos

**Projeto:** Sistema de Gerenciamento de Tarefas  
**Cliente:** Equipe de Vendas - TaskFlow Inc.  
**Solicitante:** Maria Silva (Gerente de Vendas)  
**Desenvolvedor:** Você  
**Prazo:** 14/04/2025  

---

## 🎯 O Problema

Nossa equipe de vendas enfrenta os seguintes desafios diários:

1. **Esquecemos tarefas importantes**
   - Não temos um lugar centralizado para anotações
   - Usamos papéis soltos que se perdem
   - Alguns usam blocos de notas diferentes

2. **Perdemos tempo**
   - Gastamos 30min por dia só organizando o que fazer
   - Não sabemos por onde começar
   - Reescrevemos listas todos os dias

3. **Falta priorização**
   - Tudo parece urgente
   - Não sabemos o que fazer primeiro
   - Fazemos coisas menos importantes

4. **Trabalho duplicado**
   - Às vezes fazemos a mesma coisa duas vezes
   - Não lembramos o que já foi feito

5. **Perda de informações**
   - Anotações em papéis que somem
   - Post-its que caem
   - Sem backup

**Impacto no negócio:**
- 🔴 Clientes sem follow-up adequado
- 🔴 Prazos de propostas perdidos
- 🔴 Produtividade 30% abaixo do esperado
- 🔴 Estresse alto na equipe
- 🔴 Perda de vendas

---

## 👥 Personas (Quem Vai Usar)

### 👨‍💼 Pedro - Vendedor Sênior (42 anos)

**Perfil:**
- 15 anos de experiência em vendas
- Gerencia 50+ tarefas por semana
- Usa computador no escritório e celular em campo
- Pouca paciência com tecnologia complicada

**Comportamento:**
- Prefere coisas simples e diretas
- Não gosta de muitos cliques
- Usa celular 70% do tempo
- Esquece facilmente se não anotar

**Frase típica:**  
> "Preciso de algo que não me atrapalhe, só me ajude! Sem firulas!"

**Necessidades:**
- Adicionar tarefa MUITO rápido
- Ver lista clara de pendentes
- Marcar como feito com 1 clique

---

### 👩‍💼 Ana - Vendedora Júnior (24 anos)

**Perfil:**
- 2 anos de experiência
- Gerencia 20-30 tarefas por semana
- Usa celular 90% do tempo
- Confortável com tecnologia

**Comportamento:**
- Gosta de coisas organizadas e bonitas
- Usa apps no dia a dia
- Valoriza experiência visual
- Metódica e organizada

**Frase típica:**  
> "Quero saber exatamente o que fazer quando abro o app! E que seja bonito, né!"

**Necessidades:**
- Interface agradável
- Organização clara
- Ver progresso visual
- Funcionar bem no celular

---

### 👨‍💻 Carlos - Coordenador de Vendas (35 anos)

**Perfil:**
- 8 anos na empresa
- Gerencia 30-40 tarefas próprias por semana
- Usa computador 100% do tempo
- Tech-savvy

**Comportamento:**
- Precisa de visão geral
- Gosta de estatísticas
- Organizado e metódico
- Toma decisões baseadas em dados

**Frase típica:**  
> "Preciso ver o progresso de forma clara. Quantas fiz hoje? Quantas faltam?"

**Necessidades:**
- Dashboard com números
- Filtros para organizar
- Visão geral rápida

---

## 💭 Histórias de Uso (User Stories)

### 📝 História 1: Adicionar Tarefa Rapidamente

COMO vendedor
QUERO adicionar tarefas rapidamente
PARA não perder ideias durante reuniões com clientes

CRITÉRIOS DE ACEITAÇÃO:
✓ Consigo adicionar em menos de 5 segundos
✓ Não preciso preencher muitos campos obrigatórios
✓ Posso adicionar pelo celular com teclado touch
✓ Input sempre visível (não preciso procurar)
✓ Funciona com Enter (não preciso clicar em botão)

**Cenário:**
> Pedro está em reunião com cliente. Cliente menciona que precisa de 
> orçamento até sexta. Pedro pega celular, abre app, digita 
> "Enviar orçamento Cliente X", aperta Enter. Pronto. 3 segundos.

---

### 👀 História 2: Ver O Que Fazer Agora

COMO vendedor
QUERO ver minhas tarefas pendentes
PARA saber no que focar agora

CRITÉRIOS DE ACEITAÇÃO:
✓ Vejo pendentes separadas de concluídas
✓ As mais recentes aparecem primeiro
✓ Visual deixa claro quais ainda não fiz
✓ Consigo alternar entre ver "todas" e "só pendentes"

**Cenário:**
> Ana chega no escritório às 9h. Abre o app. Clica em "Pendentes".
> Vê 8 tarefas que precisa fazer. Escolhe a primeira e começa.

---

### ✅ História 3: Marcar Como Concluída

COMO vendedor
QUERO marcar tarefas como concluídas
PARA ter satisfação de ver meu progresso

CRITÉRIOS DE ACEITAÇÃO:
✓ Marcar/desmarcar com 1 clique
✓ Visual muda claramente (riscado, cor diferente)
✓ Vejo quantas já completei
✓ Tarefas concluídas não desaparecem (posso ver depois)

**Cenário:**
> Pedro termina de enviar proposta. Clica no checkbox da tarefa.
> Tarefa fica riscada. Contador mostra "5 concluídas hoje". Pedro sorri.

---

### ✏️ História 4: Corrigir Erro em Tarefa

COMO vendedor
QUERO editar tarefas que digitei errado
PARA corrigir informações sem ter que deletar e recriar

CRITÉRIOS DE ACEITAÇÃO:
✓ Botão de editar visível em cada tarefa
✓ Posso modificar o texto
✓ Posso cancelar edição se quiser
✓ Não perco a tarefa se errar na edição

**Cenário:**
> Ana digitou "Ligar para João" mas era "Ligar para José".
> Clica em editar, muda o nome, salva. Simples.

---

### 🗑️ História 5: Deletar Tarefas Desnecessárias

COMO vendedor
QUERO deletar tarefas que não fazem mais sentido
PARA manter minha lista limpa e relevante

CRITÉRIOS DE ACEITAÇÃO:
✓ Botão de deletar em cada tarefa
✓ Sistema pede confirmação (não deleta acidentalmente)
✓ Tarefa some da lista após deletar

**Cenário:**
> Carlos criou tarefa "Ligar para Cliente X". Cliente cancelou contrato.
> Tarefa não faz mais sentido. Clica em deletar, confirma, some da lista.

---

### 🔍 História 6: Encontrar Tarefa Específica

COMO vendedor
QUERO buscar tarefas pelo texto
PARA encontrar rapidamente algo específico

CRITÉRIOS DE ACEITAÇÃO:
✓ Campo de busca visível
✓ Busca enquanto digito (tempo real)
✓ Não diferencia maiúsculas/minúsculas
✓ Mostra "nenhuma encontrada" se não achar

**Cenário:**
> Pedro tem 50 tarefas. Precisa achar aquela sobre "Proposta Empresa Y".
> Digita "empresa y" na busca. Aparece só essa tarefa. Encontrou em 2 segundos.

---

### 📊 História 7: Ver Meu Progresso

COMO vendedor
QUERO ver estatísticas das minhas tarefas
PARA saber se estou sendo produtivo

CRITÉRIOS DE ACEITAÇÃO:
✓ Vejo total de tarefas
✓ Vejo quantas estão pendentes
✓ Vejo quantas já concluí
✓ Números atualizam automaticamente

**Cenário:**
> Carlos abre o app. Vê "Total: 25 | Pendentes: 8 | Concluídas: 17".
> Sabe que já fez mais da metade. Motivado, continua trabalhando.

---

### 🧹 História 8: Limpar Tarefas Antigas

COMO vendedor
QUERO deletar todas as concluídas de uma vez
PARA não ter que deletar uma por uma no fim da semana

CRITÉRIOS DE ACEITAÇÃO:
✓ Botão "Limpar Concluídas" visível
✓ Deleta todas as marcadas como concluídas
✓ Pede confirmação antes de deletar
✓ Pendentes não são afetadas

**Cenário:**
> Sexta-feira, fim do dia. Ana tem 30 tarefas concluídas acumuladas.
> Clica em "Limpar Concluídas". Confirma. Todas somem. Lista limpa para segunda.

---

### 💾 História 9: Não Perder Minhas Tarefas

COMO vendedor
QUERO que minhas tarefas sejam salvas automaticamente
PARA não perder tudo se fechar o navegador por acidente

CRITÉRIOS DE ACEITAÇÃO:
✓ Tarefas são salvas automaticamente
✓ Quando volto ao app, minhas tarefas estão lá
✓ Funciona mesmo se fechar navegador
✓ Funciona mesmo se desligar computador

**Cenário:**
> Pedro adiciona 5 tarefas. Navegador trava. Ele reinicia.
> Abre o app de novo. As 5 tarefas estão lá. Nada perdido.

---

### 📱 História 10: Usar no Celular

COMO vendedora que trabalha em campo
QUERO que o app funcione perfeitamente no celular
PARA gerenciar tarefas onde quer que eu esteja

CRITÉRIOS DE ACEITAÇÃO:
✓ Todos os botões são grandes o suficiente para tocar
✓ Layout se adapta à tela pequena
✓ Não preciso dar zoom
✓ Teclado do celular não esconde conteúdo importante

**Cenário:**
> Ana está no carro entre duas reuniões. Pega celular, abre app,
> adiciona tarefa com teclado touch. Tudo funciona perfeitamente.

---

## 🎨 Expectativas Visuais

### O Que Queremos Ver:

**✅ Design Profissional**
- Limpo e organizado
- Não parece "projeto de escola"
- Cores agradáveis e profissionais
- Fonte legível (não muito pequena!)

**✅ Visual Claro**
- Fácil distinguir tarefas pendentes de concluídas
- Botões óbvios (não precisa adivinhar o que fazem)
- Feedback visual para todas ações
- Estados hover/focus visíveis

**✅ Responsivo**
- Bonito no desktop
- Bonito no tablet
- Bonito no celular
- Tudo acessível em qualquer tela

**❌ O Que NÃO Queremos:**
- Design amador ou "feio"
- Cores berrantes ou sem harmonia
- Texto muito pequeno
- Botões minúsculos no mobile
- Layout quebrado em alguma tela

---

## 🚫 O Que NÃO Precisamos (Pelo Menos Agora)

Para este primeiro MVP (Produto Mínimo Viável), **NÃO** precisamos de:

- ❌ Login/Cadastro de usuários
- ❌ Compartilhar tarefas entre pessoas
- ❌ Notificações push
- ❌ Sincronização na nuvem
- ❌ Categorias/tags (seria legal, mas não é essencial)
- ❌ Prioridades (seria legal, mas não é essencial)
- ❌ Datas de vencimento (seria legal, mas não é essencial)
- ❌ Anexos/fotos
- ❌ Comentários
- ❌ Histórico de alterações

**Foco:** Fazer o básico MUITO BEM FEITO!

---

## 📝 Requisitos Técnicos (Resumo)

### O Que Você DEVE Usar:

✅ **HTML5** - Estrutura semântica  
✅ **CSS3** - Estilização própria (sem frameworks)  
✅ **JavaScript Puro** - Sem bibliotecas/frameworks  
✅ **LocalStorage** - Para salvar dados  

### O Que Você NÃO PODE Usar:

❌ React, Vue, Angular  
❌ Bootstrap, Tailwind  
❌ jQuery  
❌ Banco de dados externo  

**Por quê?** Queremos avaliar seus fundamentos!

---

## ✅ Critérios de Sucesso

### Para a Equipe de Vendas Aprovar, o App Precisa:

1. **Funcionar** - Todas as funcionalidades principais operacionais
2. **Ser rápido** - Adicionar tarefa em menos de 5 segundos
3. **Ser intuitivo** - Qualquer pessoa consegue usar sem manual
4. **Ser bonito** - Design profissional, não amador
5. **Ser responsivo** - Funcionar em desktop E celular
6. **Ser confiável** - Não perder dados

### Para Você Ser Aprovado, o Código Precisa:

1. **Estar no GitHub** - Repositório público
2. **Estar online** - Deploy funcionando
3. **Ter README** - Documentação completa
4. **Ser limpo** - Organizado e comentado
5. **Seguir padrões** - HTML semântico, CSS organizado, JS estruturado

---

## 🎯 Definição de Pronto (Definition of Done)

Uma funcionalidade só está "pronta" quando:

- [ ] Código escrito e funcionando
- [ ] Testado em desktop
- [ ] Testado em mobile
- [ ] Testado em Chrome e Firefox
- [ ] Sem erros no console
- [ ] Código commitado no GitHub
- [ ] Funciona na versão online (deploy)

---

## 💬 Feedback da Equipe (Simulado)

**Pedro disse:**
> "Olha, eu não entendo nada de tecnologia, mas preciso que seja
> MUITO fácil de usar. Se eu precisar de tutorial, não serve."

**Ana disse:**
> "Eu uso vários apps no celular. O meu parâmetro é: se for mais
> difícil que Instagram, está complicado demais!"

**Carlos disse:**
> "Preciso confiar que meus dados não vão sumir. E preciso ver
> meu progresso, saber se estou produzindo ou enrolando."

**Maria (sua gestora) disse:**
> "Capriche! Este projeto vai para seu portfólio e pode ser
> o diferencial na sua carreira. Mostre do que você é capaz!"

---

## 🎊 Resultado Esperado

**Quando você entregar este projeto, você terá:**

1. ✅ Seu primeiro projeto profissional completo
2. ✅ Algo real para colocar no portfólio
3. ✅ Experiência de trabalhar com "cliente real"
4. ✅ Prática com todas as tecnologias do curso
5. ✅ Um app que pessoas reais vão usar
6. ✅ Confiança para o próximo desafio

**A equipe de vendas terá:**

1. ✅ Ferramenta para organizar tarefas
2. ✅ Mais produtividade
3. ✅ Menos estresse
4. ✅ Mais vendas (esperamos!)

---

## 🤝 Combinados

### Você tem autonomia para:

- ✅ Escolher cores e design (desde que profissional)
- ✅ Decidir posicionamento de elementos
- ✅ Adicionar funcionalidades extras (se quiser)
- ✅ Implementar do jeito que achar melhor

### Mas precisa garantir:

- ✅ Todas as funcionalidades obrigatórias
- ✅ Funcionar em mobile
- ✅ Código de qualidade
- ✅ Prazo respeitado

### Se tiver dúvidas:

- 💬 Discord DevMode (time de desenvolvimento)
- 📧 maria.silva@taskflow.com (cliente)
- 👥 Colegas de equipe (outros devs)

---

## 🎯 Última Palavra da Maria


"Sei que pode parecer desafiador, mas você foi contratado porque
acreditamos no seu potencial.

Este projeto vai mostrar do que você é capaz. Não precisa ser perfeito,
precisa ser funcional e bem feito.

Estamos aqui para apoiar. Pergunte quando precisar.

Você consegue! 💪

Boa sorte!

- Maria"


---

## 🚀 Agora É Com Você!

Você tem todos os requisitos.  
Você tem o apoio da equipe.  
Você tem o prazo.  

**Hora de colocar a mão na massa e mostrar seu valor!**

**Transforme este briefing em realidade.  
Mostre que você é um(a) Dev Júnior de verdade!**

---

**Bora codar! 💻🔥**

---

*Este é um projeto fictício criado para fins educacionais do curso DevMode 2025.*  
*Qualquer semelhança com empresas reais é mera coincidência.*
```
