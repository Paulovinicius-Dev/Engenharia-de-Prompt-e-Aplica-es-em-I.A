# Aula 03 — Desmontando a Máquina e Desbloqueando o Raciocínio

## 📚 Objetivo da Aula
Nesta atividade exploramos como modelos de linguagem funcionam internamente a partir de dois conceitos importantes:

- **Tokenização** (como o texto é dividido para o modelo entender)
- **Previsão de palavras** (como o modelo decide qual palavra vem depois)
- **Raciocínio estruturado (Chain-of-Thought)** para resolver problemas passo a passo.

---

# 🔎 Etapa 1 — Análise de Tokens

Utilizamos o **OpenAI Tokenizer** para analisar como a frase é quebrada em tokens.

### Resultado
- Número total de tokens: *(preencher com o resultado obtido)*
- Observação: palavras podem ser divididas em partes menores chamadas **tokens**, que nem sempre correspondem exatamente às palavras completas.

### Print da análise

<img width="734" height="863" alt="Captura de tela 2026-03-09 213714" src="https://github.com/user-attachments/assets/50b9e970-6751-444c-b965-a7e572aaa938" />

---

# 🤖 Etapa 2 — Teste de Previsibilidade

Prompt utilizado: "O gato come..." liste 3 palavras provaveis com justificativa lógicas e simule diferentes temperaturas sendo muito criativa vs muito técnica.

Foi solicitado que a IA previsse as **3 palavras mais prováveis** para completar a frase.

### Resultado

Exemplo de possíveis respostas:

1. ração  
2. peixe  
3. comida  

### Justificativa

O modelo escolhe palavras baseadas em **probabilidade estatística**, analisando grandes volumes de texto usados durante o treinamento. Como "gato" frequentemente aparece associado a comida, ração ou peixe, essas palavras têm maior probabilidade de aparecer.

Também simulamos dois estilos:

- **Modo criativo** → respostas mais variadas
- **Modo técnico** → respostas mais previsíveis e diretas

### Print do teste

<img width="891" height="912" alt="Captura de tela 2026-03-09 212436" src="https://github.com/user-attachments/assets/672eb98d-22e5-4b9f-9d95-6dfb7dfe74b9" />

<img width="940" height="910" alt="Captura de tela 2026-03-09 212455" src="https://github.com/user-attachments/assets/cf46ded8-67df-4f37-8a3e-1d607bdb172c" />

---

# 🧠 Etapa 3 — Desbloqueando o Raciocínio (Chain-of-Thought)

Desafio proposto:

> Qual é a terceira letra da quinta palavra da frase  
> **"O rato roeu a roupa do Rei de Roma?"**

### Resolução passo a passo

Frase separada em palavras:

1. O  
2. rato  
3. roeu  
4. a  
5. roupa  
6. do  
7. Rei  
8. de  
9. Roma  

A **quinta palavra** é: **u**


### Print do teste

<img width="924" height="742" alt="Captura de tela 2026-03-09 212502" src="https://github.com/user-attachments/assets/a3b1fdf2-3f24-4d72-b1c4-46fa65f2a1f9" />

---

# 📊 Conclusão

A atividade demonstrou que os modelos de linguagem funcionam a partir de **tokens e probabilidades**, e não necessariamente de compreensão semântica humana.

Observamos que:

- A **tokenização influencia diretamente** como a IA interpreta o texto.
- A previsão de palavras ocorre com base em **probabilidades estatísticas**.
- Ao solicitar **raciocínio passo a passo (Chain-of-Thought)**, conseguimos melhorar a precisão da resposta da IA em tarefas lógicas.

Portanto, a forma como estruturamos o **prompt** pode impactar significativamente o resultado obtido, tornando a engenharia de prompts uma habilidade importante para utilizar LLMs de forma eficiente.

---

✍️ **Autor:**  
Paulo Vinicius da Silva sousa 

📅 **Disciplina:**  
Engenharia de Prompt e Aplicações em IA

💻 **Repositório:**  
Aula 03





