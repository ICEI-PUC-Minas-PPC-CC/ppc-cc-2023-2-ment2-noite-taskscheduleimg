# Sprint 1

## Introdução ao CLU

Criamos duas "intenções" - que são ações que desejamos realizar. No nosso caso, definimos duas intenções: uma para ligar um dispositivo e outra para desligar um dispositivo. Uma intenção é como um objetivo ou tarefa que o nosso programa de computador deve compreender e executar.

Para cada uma dessas intenções, especificamos "enunciados de exemplo" que indicam o tipo de linguagem que as pessoas usam para expressar essas intenções. 

Além disso, criamos as "entidades". Entidades são detalhes ou informações específicas dentro dos enunciados que podem ser importantes para realizar a ação corretamente. Por exemplo, se alguém disser "Ligue a luz da sala de estar", a entidade aqui é "sala de estar". Ela nos diz qual luz deve ser ligada. Portanto, entidades ajudam o programa a entender e executar as intenções de maneira mais precisa.

Em resumo, o que fizemos foi criar intenções para ligar e desligar dispositivos, fornecer exemplos de como as pessoas podem expressar essas intenções e mencionar entidades para capturar informações relevantes. Isso é útil em desenvolvimento de software para entender e responder às solicitações dos usuários de forma eficaz.

### Criação das intenções, enunciados e entidades
---
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/be8add31-9c25-4884-b7ef-0292266b92e5)
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/223012b4-386e-47ec-92eb-113978d4a598)
---
### Depois, treinamos o modelo com as intenções, enunciados e entidades definidas.
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/961c3dc7-4407-4f54-989d-88a1c044a82f)
---
### Acompanhamos o resultado do treinamento pra acompanhar a assertividade do treinamento.
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/c9316d5e-39f9-4240-b971-2cc9ceb5f767)
---
### Implantamos o modelo previamente treinado para os testes.
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/05eb8f3a-e045-4717-b03e-1cc4aad72ddd)

-------
### Primeiro Teste:
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/222e26ab-76ee-4b49-b7ca-f7d17454cb66)

#### Código do teste:
````
{
    "query": "desligue a luz da sala",
    "prediction": {
        "topIntent": "desligar_interruptor",
        "projectKind": "Conversation",
        "intents": [
            {
                "category": "desligar_interruptor",
                "confidenceScore": 0.96083486
            },
            {
                "category": "ligar_interruptor",
                "confidenceScore": 0.93714297
            },
            {
                "category": "None",
                "confidenceScore": 0
            }
        ],
        "entities": [
            {
                "category": "dispositivo",
                "text": "luz",
                "offset": 11,
                "length": 3,
                "confidenceScore": 1
            },
            {
                "category": "lugar",
                "text": "sala",
                "offset": 18,
                "length": 4,
                "confidenceScore": 1
            }
        ]
    }
}
````

---
### Segundo teste:
![image](https://github.com/ICEI-PUC-Minas-PPC-CC/ppc-cc-2023-2-ment2-noite-taskscheduleimg/assets/143455854/5794a332-e516-42f8-9d78-97a5318d42d0)

#### Código do teste:
````
{
    "query": "ligue a caixa de música no hospital",
    "prediction": {
        "topIntent": "ligar_interruptor",
        "projectKind": "Conversation",
        "intents": [
            {
                "category": "ligar_interruptor",
                "confidenceScore": 0.927994
            },
            {
                "category": "desligar_interruptor",
                "confidenceScore": 0.8716618
            },
            {
                "category": "None",
                "confidenceScore": 0
            }
        ],
        "entities": [
            {
                "category": "dispositivo",
                "text": "caixa de música",
                "offset": 8,
                "length": 15,
                "confidenceScore": 1
            },
            {
                "category": "lugar",
                "text": "hospital",
                "offset": 27,
                "length": 8,
                "confidenceScore": 1
            }
        ]
    }
}
````
