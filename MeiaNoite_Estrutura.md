# Meia Noite - Estrutura Musical e Dinâmica

---

## 1. Roteiro Sequencial da Bateria (Flowchart)

```mermaid
flowchart TD
    V1["<b>Verso 1</b><br>Bumbo suave"] 
    --> V2["<b>Verso 2</b><br>1. Bumbo + Cx + Surdo<br>2. Bumbo dobra + Cx + Pratos abertos"]
    --> PR1["<b>Pré-Refrão</b><br>Bumbo + Chimbal + Cx + Surdo"]
    --> R1["<b>Refrão</b><br>Groove Extremo (Todas as batidas)"]
    --> V1_2["<b>Verso</b><br>Groove direto ... Pausa"]
    --> PR2["<b>Pré-Refrão</b><br>Groove + Tons"]
    --> R2["<b>Refrão</b><br>Groove"]
    --> P["<b>Ponte</b><br>Rufi + Tons"]
    --> RF["<b>Refrão Final</b><br>Groove Quebrado"]
```

---

## 2. Visão em Blocos por Fases (Horizontal)

```mermaid
flowchart LR
    subgraph Bloco1["Parte 1: Construção"]
        A1["Verso 1<br>(Bumbo suave)"] --> A2["Verso 2<br>(Dobra)"] --> A3["Pré-Refrão<br>(Condução)"] --> A4["Refrão 1<br>(Extremo)"]
    end

    subgraph Bloco2["Parte 2: Dinâmica e Reprise"]
        B1["Verso<br>(Pausa)"] --> B2["Pré-Refrão<br>(+ Tons)"] --> B3["Refrão 2<br>(Groove)"]
    end

    subgraph Bloco3["Parte 3: Clímax"]
        C1["Ponte<br>(Rufi + Tons)"] --> C2["Refrão Final<br>(Groove Quebrado)"]
    end

    Bloco1 --> Bloco2 --> Bloco3
```

---

## 3. Mapa de Transição e Intensidade (State Diagram)

```mermaid
stateDiagram-v2
    [*] --> Verso1 : Suave
    Verso1 --> Verso2 : Entrada de Bumbo, Cx e Surdo
    Verso2 --> PréRefrão1 : Condução com Chimbal
    PréRefrão1 --> Refrão1 : Groove Extremo (Intensidade Máxima)
    Refrão1 --> Verso2_Pausa : Quebra com Pausa
    Verso2_Pausa --> PréRefrão2 : Crescendo com Tons
    PréRefrão2 --> Refrão2 : Groove Firme
    Refrão2 --> Ponte : Rufi + Tons
    Ponte --> RefrãoFinal : Groove Quebrado (Finalização)
    RefrãoFinal --> [*]
```
