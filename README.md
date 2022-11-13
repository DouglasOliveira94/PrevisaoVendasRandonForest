# Mentorama Model API

Modelo treinado utilizando uma random forest. 

### Rotas
- POST
    ```/predict:``` versão final do modelo para previsão
        
        model inputs:
            -  X1: Valor de Marketing investindo em TV
            -  X2: Valor de Marketing investindo em Radio
            -  X3: Valor de Marketing investindo em jornal

        model output: 
        prediction: valor que será retornado em vendas em Milhares de reais

- GET
    ```/model_health/<model_id>```: Metricas do modelo. Recall e Precision disponíveis. 
        
        model_id: id do modelo em produção
