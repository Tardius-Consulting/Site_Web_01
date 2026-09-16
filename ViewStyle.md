# 🎨 Guia de Identidade Visual & Estilo Front-End | Lotl SaaS

Este guia estabelece as especificações visuais de Front-End (UI/UX) para o desenvolvimento do site institucional do **Lotl**. O layout adota uma abordagem **Light Mode** convidativa com fundo opaco suave (`#EEEEEE`) e cartões em branco puro (`#FFFFFF`), combinando o tom tecnológico com uma navegação leve.

---

## 1. Paleta de Cores do Front-End

| Nome | Hexadecimal | Elemento / Aplicação na UI |
| :--- | :--- | :--- |
| **Background Principal** | `#EEEEEE` | Fundo geral da página (`body`). Mantém o site leve e limpo. |
| **Superfície / Cards** | `#FFFFFF` | Containers, cards de recursos, depoimentos e tabela de preços. |
| **Rosa Suave (Primária)** | `#FF82A9` | Cor principal da marca. Aplicada em CTAs de conversão, logos e destaques. |
| **Escuro Profundo** | `#12151E` | Títulos (H1, H2), textos principais, botões primários e rodapé. |
| **Escuro Secundário** | `#1A1F2C` | Header/Nav superior, barras de código ou cards com contraste. |
| **Ciano Brilhante** | `#5CE1E6` | Links, badges da IA, ícones interativos e detalhes visuais. |
| **Verde Sucesso** | `#55DD55` | Checkmarks de planos, badges de confirmação e tag *"Mais Popular"*. |
| **Vermelho Alerta** | `#FF5964` | Validações de formulário, avisos de erro e exclusões. |

---

## 2. Tipografia e Hierarquia de Texto

* **Fonte Principal (Interface):** `Inter`, `Roboto` ou Sans-serif equivalente.
* **Fonte Secundária (Automação/Código):** `Fira Code`, `JetBrains Mono` ou Monospaced equivalente.

### CSS de Exemplo para Tipografia

```css
/* Título Principal (Hero Section) */
h1 {
  font-family: 'Inter', sans-serif;
  font-size: 40px;
  font-weight: 800;
  color: #12151E;
}

/* Destaque no H1 */
h1 span {
  color: #FF82A9;
}

/* Subtítulos de Seções */
h2 {
  font-family: 'Inter', sans-serif;
  font-size: 24px;
  font-weight: 700;
  color: #12151E;
  border-left: 4px solid #FF82A9;
  padding-left: 10px;
}

/* Corpo de Texto (Body) */
p {
  font-family: 'Inter', sans-serif;
  font-size: 15px;
  line-height: 1.6;
  color: #333333;
}

/* Blocos de Script / Automação */
code, pre {
  font-family: 'Fira Code', monospace;
  font-size: 13px;
  color: #008085;
}
```
## 3. Regras de Layout e Botões (CTAs)

### ☀️ Estrutura Light (`body: #EEE`)
* O `body` da página deve utilizar o background `#EEEEEE`.
* Para criar profundidade sem poluir o visual, todos os cards de conteúdo (como a Tabela de Preços e o FAQ) devem ser brancos (`#FFFFFF`) com cantos arredondados (`border-radius: 8px` ou `12px`) e sombra sutil (`box-shadow: 0 4px 12px rgba(0,0,0,0.04)`).

### 🔘 Estilização dos Botões (CTAs)
* **CTA Principal ("Comece Grátis" / "Testar Pro"):**
  * Background: `#FF82A9`
  * Cor do Texto: `#12151E` (Bold)
  * Border Radius: `6px`
  * Hover: Aumento sutil de brilho/elevação (`transform: translateY(-2px)`).
* **CTA Secundário ("Ver Planos"):**
  * Background: Transparente
  * Borda: `2px solid #12151E` ou `#FF82A9`
  * Cor do Texto: `#12151E`

---

## 4. Componentes Específicos do SaaS

* **Cards de Recursos (Home):**
  * Fundo `#FFFFFF` com borda de `1px solid #E5E5E5`.
  * Ícones destacados na cor `#FF82A9`.
* **Tabela de Planos (Preços):**
  * O card do **Plano Pro** deve ter uma borda em destaque de `2px solid #FF82A9` e uma badge `<span class="badge">MAIS POPULAR</span>` em `#FF82A9` com texto `#12151E`.
* **Accordion do FAQ:**
  * Fundo `#FFFFFF` com linhas divisórias em `#EEEEEE`.
  * Ao expandir a pergunta, o título deve ganhar destaque em `#FF82A9`.