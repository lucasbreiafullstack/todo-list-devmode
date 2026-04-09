# 📖 Instruções Detalhadas - TaskFlow

## 🗺️ Guia Passo a Passo

Este documento contém o passo a passo completo para desenvolver o projeto.

---

## 📍 FASE 1: Setup Inicial (15min)

### 1. Clone e Configure
```bash
# 1. Clone o repositório
git clone https://github.com/devmode-curso/taskflow-projeto-devmode.git
cd taskflow-projeto-devmode

# 2. Crie sua branch
git checkout -b seu-nome

# 3. Remova origin e adicione seu repo
git remote remove origin
git remote add origin https://github.com/SEU-USUARIO/taskflow-seu-nome.git

# 4. Primeiro push
git add .
git commit -m "chore: setup inicial"
git push -u origin seu-nome
```

### 2. Planejamento

Antes de começar a codar:

- [ ] Leia TODOS os requisitos em RUBRICA.md
- [ ] Faça sketch no papel da interface
- [ ] Liste funcionalidades por prioridade
- [ ] Defina estrutura de dados (como será cada tarefa)

**Tempo sugerido: 15 minutos**

---

## 📍 FASE 2: HTML (30min)

### O que criar:
```html
<!-- Estrutura básica -->
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <!-- Meta tags -->
    <!-- Title -->
    <!-- Link CSS -->
</head>
<body>
    <header>
        <!-- Logo e título -->
    </header>
    
    <main>
        <!-- Formulário de nova tarefa -->
        <section class="add-task">
            <form>
                <input type="text" placeholder="Nova tarefa...">
                <button>Adicionar</button>
            </form>
        </section>
        
        <!-- Controles (filtros e busca) -->
        <section class="controls">
            <!-- Filtros -->
            <!-- Busca -->
        </section>
        
        <!-- Estatísticas -->
        <section class="stats">
            <!-- Contadores -->
        </section>
        
        <!-- Lista de tarefas -->
        <section class="tasks">
            <ul id="listaTarefas">
                <!-- Tarefas via JS -->
            </ul>
        </section>
    </main>
    
    <footer>
        <!-- Créditos -->
    </footer>
    
    <script src="js/script.js"></script>
</body>
</html>
```

### Checklist:

- [ ] DOCTYPE e meta tags
- [ ] Tags semânticas (header, main, section, footer)
- [ ] Formulário com label
- [ ] IDs e classes apropriados
- [ ] Comentários organizando

**Commit**: `feat: estrutura HTML completa`

---

## 📍 FASE 3: CSS Base (45min)

### 3.1 Reset e Variáveis (10min)
```css
/* Reset */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

/* Variáveis */
:root {
    --primary: #6366f1;
    --bg-body: #f8fafc;
    --text: #1e293b;
    /* ... mais variáveis */
}
```

**Commit**: `style: reset CSS e variáveis`

### 3.2 Layout Geral (15min)

- Container
- Header
- Main
- Footer

**Commit**: `style: layout base`

### 3.3 Componentes (20min)

- Formulário
- Botões
- Cards de tarefa
- Filtros
- Busca

**Commit**: `style: componentes principais`

---

## 📍 FASE 4: JavaScript - CRUD Básico (60min)

### 4.1 Estrutura e Estado (10min)
```javascript
// Estado
let tarefas = [];

// Elementos DOM
const form = document.querySelector('#form');
const input = document.querySelector('#input');
const lista = document.querySelector('#lista');

// Inicialização
function init() {
    carregarTarefas();
    renderizar();
    eventos();
}

document.addEventListener('DOMContentLoaded', init);
```

**Commit**: `feat: estrutura JS e estado inicial`

### 4.2 Adicionar Tarefa (15min)
```javascript
function adicionarTarefa(texto) {
    const novaTarefa = {
        id: Date.now(),
        texto: texto,
        concluida: false,
        data: new Date().toISOString()
    };
    
    tarefas.unshift(novaTarefa);
    salvar();
    renderizar();
}
```

**Commit**: `feat: adicionar tarefa`

### 4.3 Renderizar Lista (15min)
```javascript
function renderizar() {
    lista.innerHTML = '';
    
    tarefas.forEach(tarefa => {
        const li = criarElemento(tarefa);
        lista.appendChild(li);
    });
    
    atualizarStats();
}

function criarElemento(tarefa) {
    // Criar li com checkbox, texto, botões
    // Retornar elemento
}
```

**Commit**: `feat: renderizar lista de tarefas`

### 4.4 Toggle e Deletar (20min)
```javascript
function toggleTarefa(id) {
    const tarefa = tarefas.find(t => t.id === id);
    tarefa.concluida = !tarefa.concluida;
    salvar();
    renderizar();
}

function deletarTarefa(id) {
    if (!confirm('Deletar?')) return;
    tarefas = tarefas.filter(t => t.id !== id);
    salvar();
    renderizar();
}
```

**Commit**: `feat: toggle e deletar tarefa`

---

## 📍 FASE 5: LocalStorage (20min)
```javascript
function salvar() {
    localStorage.setItem('tarefas', JSON.stringify(tarefas));
}

function carregar() {
    const dados = localStorage.getItem('tarefas');
    return dados ? JSON.parse(dados) : [];
}

function carregarTarefas() {
    tarefas = carregar();
}
```

**Commit**: `feat: persistência com LocalStorage`

---

## 📍 FASE 6: Funcionalidades Avançadas (60min)

### 6.1 Editar Tarefa (20min)

**Commit**: `feat: editar tarefa`

### 6.2 Filtros (15min)

**Commit**: `feat: filtros (todas/pendentes/concluídas)`

### 6.3 Busca (15min)

**Commit**: `feat: busca em tempo real`

### 6.4 Limpar Concluídas (10min)

**Commit**: `feat: limpar tarefas concluídas`

---

## 📍 FASE 7: Responsividade (30min)

### Media Queries
```css
/* Mobile First */
@media (min-width: 768px) {
    /* Tablet */
}

@media (min-width: 1200px) {
    /* Desktop */
}
```

**Commit**: `style: responsividade completa`

---

## 📍 FASE 8: Polimento (30min)

- Animações
- Transições
- Estados vazios
- Mensagens de feedback

**Commit**: `style: animações e polish final`

---

## 📍 FASE 9: README (30min)

Use o template em `templates/README-TEMPLATE.md`

- [ ] Título e descrição
- [ ] Screenshot
- [ ] Funcionalidades
- [ ] Tecnologias
- [ ] Como usar
- [ ] Link do deploy

**Commit**: `docs: README completo`

---

## 📍 FASE 10: Deploy (20min)

### GitHub Pages:
```bash
# 1. Push para GitHub
git push

# 2. No GitHub:
# Settings → Pages → Source: main branch → Save

# 3. Aguardar 2-3 minutos
# 4. Acessar: https://seu-usuario.github.io/taskflow-seu-nome
```

### Netlify (alternativa):

1. Arraste pasta do projeto em netlify.com
2. Pronto!

**Commit**: `chore: configuração de deploy`

---

## 🎯 Dicas Importantes

### ✅ FAÇA:

- Commits pequenos e frequentes
- Teste após cada funcionalidade
- Leia a documentação (MDN)
- Peça ajuda no Discord
- Comece cedo

### ❌ EVITE:

- Copiar código completo
- Deixar para última hora
- Ignorar mobile
- Pular testes
- Commit gigante no final

---

## 🆘 Troubleshooting

### "LocalStorage não salva"
```javascript
// Sempre usar try/catch
try {
    localStorage.setItem('tarefas', JSON.stringify(tarefas));
} catch (error) {
    console.error('Erro ao salvar:', error);
}
```

### "Tarefa não deleta"
```javascript
// Verificar se está removendo do array E salvando
tarefas = tarefas.filter(t => t.id !== id);
salvar(); // ← NÃO ESQUECER!
renderizar();
```

### "CSS não carrega"
```html
<!-- Verificar caminho -->
<link rel="stylesheet" href="css/style.css">
<!-- Não: -->
<!-- <link rel="stylesheet" href="style.css"> -->
```

---

**Boa sorte! 🚀**
