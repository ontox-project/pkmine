## A method description for slide 

![imaging-conference](https://github.com/ontox-project/pkmine/assets/12751032/6f396739-4aba-4d28-9a14-a1444ac5033a)


Via GPT-4o:

PROMPT - AI response:

Me: Convert the diagram that depicts a PBPK model to mermaid syntax.

ChatGPT:
To convert the diagram depicting a PBPK (Physiologically Based Pharmacokinetic) model to mermaid syntax, we need to create a flowchart that illustrates the key elements and connections shown in the image.

Here's the mermaid code for the PBPK model based on the provided diagram:

```mermaid

graph TD
    A[In vitro Data] -->|Absorption| B1[Lungs]
    A -->|Absorption| B2[GI tract]
    A -->|Distribution| C1[Blood]
    A -->|Distribution| C2[Fat]
    A -->|Distribution| C3[Rapidly perfused tissue]


    A -->|Distribution| C4[Slowly perfused tissue]
    A -->|Metabolism| D1[Liver]
    A -->|Excretion| E1[Kidney minus PT]
    E1 -->|Filtrate| E2[Proximal Tubule]
    
    B1 --> F[% humans with adverse outcome]
    B2 --> F
    C1 --> F
    C2 --> F
    C3 --> F
    C4 --> F
    D1 --> F
    E2 --> F
    
    F --> G[External dose in humans]
    G --> H[Risk/RfD]

    %% Additional parameters
    subgraph Parameters
        Papp[P<sub>app</sub>]
        CLint[CL<sub>int</sub>]
        Vmax[V<sub>max</sub>]
    end
    
    A --> Parameters

```
