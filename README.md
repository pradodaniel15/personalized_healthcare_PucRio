# 🧬 Análise e Pré-processamento de Dados de Saúde com Dispositivos Vestíveis

Este projeto tem como objetivo realizar uma análise exploratória e o pré-processamento de um conjunto de dados de monitoramento de saúde personalizado, coletado por sensores vestíveis em diferentes ambientes e horários.

---

## 🎯 Objetivo

- Explorar padrões fisiológicos e comportamentais dos usuários
- Preparar os dados para aplicações de aprendizado de máquina
- Aplicar técnicas de transformação como normalização, padronização, discretização e codificação

---

## 📁 Estrutura do Notebook

O notebook está dividido nas seguintes seções:

1. **Definição do Problema**
2. **Análise Exploratória de Dados**
3. **Pré-processamento de Dados**
   - Conversão de tipos
   - Normalização (Min-Max)
   - Padronização (Z-score)
   - Discretização (Binning)
   - One-Hot Encoding
4. **Nova Análise Exploratória com Dados Transformados**
5. **Conclusão e próximos passos**

---

## 📊 Dataset

O dataset contém 4.500 registros e 18 atributos, incluindo:

- Sinais vitais: frequência cardíaca, temperatura corporal, oxigenação, respiração
- Atividade física, sono, passos, localização
- Variável-alvo: `activity_label` (atividade realizada)

---

## 🔗 Como carregar o dataset no notebook

Você pode carregar o dataset diretamente do GitHub usando o link raw:

```python
import pandas as pd

url = "https://raw.githubusercontent.com/pradodaniel15/personalized_healthcare_PucRio/refs/heads/main/personalized_healthcare_dataset.csv"
df = pd.read_csv(url)
