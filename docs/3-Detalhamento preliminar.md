# Detalhamento preliminar

## Projeto de Interface

COMO O C.L.U funciona: 

O CLU oferece um conjunto de domínios predefinidos que podem ajudar você a começar a criar seu aplicativo. Um aplicativo de domínio predefinido já está preenchido com intenções, entidades e enunciados.
Depois que o aplicativo for preenchido com intenções, entidades e enunciados, você precisará treinar o aplicativo para que as alterações feitas possam ser refletidas.

Após o C.L.U ter sido treinado com intenções, entidades e enunciados o mesmo começará a verificar em seu banco de dados o que mais se aproxima com o que a persona digitou. Abaixo está um exemplo de como o mesmo funciona, levando em 
consideração o chamado de "desligar a luz da sala":
````
{
    "query": "turn off the living room light",
    "prediction": {
        "topIntent": "HomeAutomation.TurnOff",
        "intents": {
            "HomeAutomation.TurnOff": {
                "score": 0.969448864
            },
            "HomeAutomation.QueryState": {
                "score": 0.0122336326
            },
            "HomeAutomation.TurnUp": {
                "score": 0.006547436
            },
            "HomeAutomation.TurnDown": {
                "score": 0.0050634006
            },
            "HomeAutomation.SetDevice": {
                "score": 0.004951761
            },
            "HomeAutomation.TurnOn": {
                "score": 0.00312553928
            },
            "None": {
                "score": 0.000552945654
            }
        },
        "entities": {
            "HomeAutomation.Location": [
                "living room"
            ],
            "HomeAutomation.DeviceName": [
                [
                    "living room light"
                ]
            ],
            "HomeAutomation.DeviceType": [
                [
                    "light"
                ]
            ],
            "$instance": {
                "HomeAutomation.Location": [
                    {
                        "type": "HomeAutomation.Location",
                        "text": "living room",
                        "startIndex": 13,
                        "length": 11,
                        "score": 0.902181149,
                        "modelTypeId": 1,
                        "modelType": "Entity Extractor",
                        "recognitionSources": [
                            "model"
                        ]
                    }
                ],
                "HomeAutomation.DeviceName": [
                    {
                        "type": "HomeAutomation.DeviceName",
                        "text": "living room light",
                        "startIndex": 13,
                        "length": 17,
                        "modelTypeId": 5,
                        "modelType": "List Entity Extractor",
                        "recognitionSources": [
                            "model"
                        ]
                    }
                ],
                "HomeAutomation.DeviceType": [
                    {
                        "type": "HomeAutomation.DeviceType",
                        "text": "light",
                        "startIndex": 25,
                        "length": 5,
                        "modelTypeId": 5,
                        "modelType": "List Entity Extractor",
                        "recognitionSources": [
                            "model"
                        ]
                    }
                ]
            }
        }
    }
}
````

Assim, é possível notar que o C.L.U compara o que foi escrito com as antigas intenções e entidades ensinadas à ele, e compara, com base na linguagem, qual mais se assemelha ao que foi pedido pelo usuário, executando a ação. Caso
a ação esteja errada, também é possível ensinar o C.L.U corretamente, prevenindo futuros erros semelhantes.

essa ação, aparentemente "simples" do C.L.U consiste em 7 etapas principais. São elas: 

1- Coleta de Dados: O CLU é treinado em uma enorme quantidade de dados de texto e áudio para aprender como as pessoas se comunicam em linguagem natural. Isso inclui textos de livros, conversas em redes sociais, gravações de áudio e muito mais.


2- Pré-processamento: Antes de entender o texto ou o áudio, o CLU faz um pré-processamento para limpar e organizar os dados. Isso inclui a remoção de pontuações, separação de palavras em tokens (unidades individuais) e a conversão de texto em um formato que o computador possa entender.

3- Análise Sintática: O CLU utiliza análise sintática para entender a estrutura gramatical das frases. Isso ajuda a identificar os sujeitos, verbos, objetos e outros elementos-chave em uma frase.

4- Análise Semântica: Além da estrutura gramatical, o CLU busca o significado das palavras e frases. Isso envolve a identificação de palavras-chave e o mapeamento delas para conceitos e entidades do mundo real. Por exemplo, ele pode entender que "Nova York" se refere a uma cidade nos Estados Unidos.

5- Aprendizado de Máquina: O CLU utiliza algoritmos de aprendizado de máquina para melhorar sua capacidade de compreensão ao longo do tempo. Ele é treinado em dados históricos e pode ajustar seus modelos com base em novos exemplos.

6- Resposta ou Ação: Depois de entender o texto ou o áudio, o CLU pode realizar ações específicas com base no que foi solicitado. Isso pode incluir responder a uma pergunta, executar uma pesquisa na internet, criar lembretes, controlar dispositivos de casa inteligente e muito mais.

7-Retorno de Informações: Por fim, o CLU retorna uma resposta ou realiza uma ação com base no que foi solicitado. Isso pode ser uma resposta em texto, uma saída de voz ou até mesmo uma ação física, dependendo do contexto e das capacidades do sistema.
## User Flow

![Exemplo de UserFlow](img/userflow.jpg)

'Como eu e meu grupo ainda não conhecemos a interface do CRC não foi possível desenvolver o User Flow adequado para o software. Conversei com o professor Diego e ele ficou de nos mandar prints e Sketchs de como funcionária a interface para que possamos trabalhar em cima.'

> **Links Úteis**:
> - [User Flow: O Quê É e Como Fazer?](https://medium.com/7bits/fluxo-de-usu%C3%A1rio-user-flow-o-que-%C3%A9-como-fazer-79d965872534)
> - [User Flow vs Site Maps](http://designr.com.br/sitemap-e-user-flow-quais-as-diferencas-e-quando-usar-cada-um/)
> - [Top 25 User Flow Tools & Templates for Smooth](https://www.mockplus.com/blog/post/user-flow-tools)
