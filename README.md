# Normalização

## 1FN

| Atributo | Tipo / Função | 
| :--- | :--- |
| Numero_DVD | Parte da Chave Primária | 
| Numero_Cliente | Parte da Chave Primária | 
| Data_Locacao | Parte da Chave Primária |
| Data_Fabricacao | Atributo Dependente Parcial de Numero_DVD |
| Titulo_Filme | Atributo Dependente Parcial de Numero_DVD |
| Estrela | Atributo Dependente Parcial / Transitivo | 
| Ano_Filmagem | Atributo Dependente Transitivo de Titulo_Filme |
| Duracao | Atributo Dependente Transitivo de Titulo_Filme | 
| Nome_Cliente | Atributo Dependente Parcial de Numero_Cliente |
| Endereco_Cliente | Atributo Dependente Parcial de Numero_Cliente |
| Data_Devolucao | Atributo Dependente Total da Chave |
| Valor_Pago | Atributo Dependente Total da Chave |

## 2FN 

### DVD_Filme_Temp
| Atributo | Tipo / Função | 
| :--- | :--- | 
| Numero_DVD | Chave Primária | 
|Data_Fabricacao | Atributo | 
| Titulo_Filme | Atributo |
| Estrela | Atributo | 
| Duracao | Atributo | |
Ano_Filmagem | Atributo |

### Cliente
| Atributo | Tipo / Função | 
| :--- | :--- | 
| Numero_Cliente | Chave Primária |
|Nome_Cliente | Atributo | 
| Endereco_Cliente | Atributo |


### Locacao
| Atributo | Tipo / Função |
| :--- | :--- | 
| Numero_DVD | Chave Primária / Chave Estrangeira | 
| Numero_Cliente | Chave Primária / Chave Estrangeira | 
| Data_Locacao | Chave Primária | 
| Data_Devolucao | Atributo | 
| Valor_Pago | Atributo |

## 3FN









