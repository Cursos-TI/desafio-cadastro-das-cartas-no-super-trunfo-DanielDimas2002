# Desafio Super Trunfo - Países - Cadastro das Cartas - Atualizado: 21/02

Bem-vindo ao desafio "Super Trunfo - Países"! No jogo Super Trunfo, os jogadores comparam os atributos das cartas para determinar a mais forte. O tema deste Super Trunfo é "Países", onde você comparará os atributos das cidades.

A empresa MateCheck contratou você para desenvolver a parte inicial do jogo, que consiste no cadastro das cartas.

O desafio está dividido em três níveis: Novato, Aventureiro e Mestre, com cada nível adicionando mais complexidade ao anterior.  **Você deve escolher qual desafio quer realizar.**

🚨 **Atenção:** O nível Novato do desafio é focado apenas no cadastro das cartas, utilizando as funções `scanf` para ler os dados e `printf` para exibi-los.

## 🎮 Nível Novato: Cadastro Básico

No nível Novato, você iniciará criando o sistema básico do jogo Super Trunfo com o tema "Países". As cartas serão divididas por estados, cada um com quatro cidades.  Imagine um país dividido em oito estados (A a H), e cada estado com quatro cidades (1 a 4).  A combinação forma o código da carta (ex: A01, B02).

🚩 **Objetivo:** Criar um programa em C que cadastra **duas** cartas com os seguintes atributos:

*   População (`int`)
*   Área (`float`)
*   PIB (`float`)
*   Número de pontos turísticos (`int`)

⚙️ **Funcionalidades do Sistema:**

*   O sistema permitirá ao usuário cadastrar os dados de **duas** cartas manualmente via terminal.
*   Após o cadastro, o sistema exibirá os dados de cada cidade de forma organizada.

📥 **Entrada** e 📤 **Saída de Dados:**

*   O usuário insere os dados de cada carta interativamente via `scanf`.
*   O programa exibe os dados cadastrados usando `printf`, com cada atributo em uma nova linha.

**Simplificações para o Nível Novato:**

*   Cadastre apenas **duas** cartas.
*   Concentre-se na leitura, armazenamento e exibição. Não implemente comparações ou outros recursos.
*   **Não use** laços (`for`, `while`) ou condicionais (`if`, `else`).


## 🛡️ Nível Aventureiro: Cálculo de Atributos

No nível Aventureiro, você expandirá o sistema para incluir o cálculo de dois novos atributos: Densidade Populacional e PIB per Capita.

🆕 **Diferença em relação ao Nível Novato:**

*   **Novos Atributos:**
    *   Densidade Populacional: População / Área (`float`)
    *   PIB per Capita: PIB / População (`float`)

⚙️ **Funcionalidades do Sistema:**

*   O sistema calculará automaticamente a Densidade Populacional e o PIB per Capita.
*   Os novos atributos serão exibidos junto com os demais.

📥 **Entrada** e 📤 **Saída de Dados:**

*   Mesma entrada do nível Novato.
*   A saída exibirá também os atributos calculados.

**Simplificações para o Nível Intermediário:**

*   Continue cadastrando apenas **duas** cartas.
*   Continue **sem usar** laços (`for`, `while`) ou condicionais (`if`, `else`).



## 🏆 Nível Mestre: Comparação e Super Poder

No nível Mestre, você implementará a comparação entre duas cartas e o cálculo do "Super Poder".

🆕 **Diferença em relação ao Nível Aventureiro:**

*   **Comparação de Cartas:** O usuário poderá comparar as duas cartas.
*   **Super Poder:** Soma de todos os atributos (inclusive os calculados), com a densidade populacional *invertida* antes da soma (1/densidade).  Tipo: `float`.

⚙️ **Funcionalidades do Sistema:**

*   Comparação atributo a atributo, mostrando qual carta venceu (1 se a Carta 1 vence, 0 se a Carta 2 vence).
*   Para Densidade Populacional, vence a carta com o *menor* valor.
*   Para os demais atributos (e o Super Poder), vence a carta com o *maior* valor.

📥 **Entrada** e 📤 **Saída de Dados:**

*   Mesma entrada dos níveis anteriores, mas a População agora é `unsigned long int`.
*   A saída mostrará o resultado da comparação para cada atributo e o Super Poder.

**Observação:**  Preste atenção à conversão de tipos ao calcular o Super Poder!

## 🏁 Conclusão

Ao concluir qualquer um dos níveis, você terá dado um passo importante no desenvolvimento do Super Trunfo - Países. Boa sorte e divirta-se programando!

Equipe de Ensino - MateCheck
content_copy

---

## ✅ Como compilar e executar o programa

### **Pré-requisitos**  
Certifique-se de que você tem o compilador `gcc` instalado.

### **Compilar o programa**
Abra o terminal na pasta onde está seu código fonte e digite:

```bash
gcc super_trunfo.c -o super_trunfo
```

### **Executar o programa**

```bash
./super_trunfo
```

---

## 🕹️ Como utilizar o programa

O programa simula uma rodada de Super Trunfo entre dois países. Você escolherá **dois atributos diferentes** para comparar.

### **Atributos disponíveis para comparação:**

1. População (milhões)  
2. Área (km²)  
3. PIB (bilhões de USD)  
4. Densidade Demográfica (hab/km²) → **Vence quem tiver o menor valor**

---

## 📋 Exemplo de uso

Ao iniciar o programa, será exibido o seguinte menu para escolher o primeiro atributo:

```
Escolha o primeiro atributo para comparar:
1 - População
2 - Área
3 - PIB
4 - Densidade Demográfica
> 
```

Após escolher, por exemplo, a opção **2 (Área)**, o menu será exibido novamente **sem repetir o atributo já escolhido**:

```
Escolha o segundo atributo para comparar:
1 - População
3 - PIB
4 - Densidade Demográfica
> 
```

Depois disso, o sistema exibirá as duas cartas e comparará os dois atributos da seguinte forma:

- Indica o valor de cada atributo em cada país.
- Calcula a soma total dos dois atributos por carta.
- Mostra qual carta venceu ou se houve empate.

---

## 🛠️ Observações

- A Densidade Demográfica segue uma regra especial: vence quem **tiver o menor valor**.
- O sistema impede que o usuário selecione o mesmo atributo duas vezes.
- O programa trata entradas inválidas com mensagens de erro e permite repetir a escolha.

---



