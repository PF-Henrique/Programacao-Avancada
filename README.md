<p align="center">
  <img alt="Wyden" src="https://github.com/PF-Henrique/Programacao-Avancada/blob/master/.docs/0.jpg" width="200px"/>
<p>


# Padrão Composite

> Aula ofertada pelo professor **Jão Ronaldo Cunha**. Resoluções feitas em aula, podem ser econtradas em **[repl.it](https://repl.it/@JoaoRonaldo/)**;  

## :memo: **Roteiro**

<div align="center">

|     :computer: topics                                   |     Description    |
|      :---                                               |      :---         |
| :heavy_check_mark: **Pattern Name and Classification**  | - Name: Composite, Classification: Estrutural|
| :heavy_check_mark: **Intent**                           |- Facilitar a implementação de objetos que se comportam como estrutura em  árvore.  |
| :heavy_check_mark: **Motivation**                       |- O Composite é um objeto projetado como uma composição de um ou mais objetos semelhantes, Todos exibindo funcionalidade semelhante. O conceito principal é que você pode manipular uma única instância do objeto da mesma forma que faria com um grupo deles|
| :heavy_check_mark: **Applicability**                    | - O Composite deve ser utilizado quando a aplicação possui alguma estrutura hierárquica e quer funcionalidades genéricas por toda a estrutura.|
| :heavy_check_mark: **Structure**                        | - O Composite tem uma estrutúra em arvore. Cada componente da mesma é explicado abaixo. |
|:heavy_check_mark:  **Participants**                     |**- Component:**
||- Declara interface para objetos da composição 
||- Implementa comportamentos padrão comuns para todas as classes 
||- Declara uma interface para acessar e gerenciar componentes filho|
||**- Leaf:**
||- Representa objetos folha da consição que não tem filhos
||- Define o comportamento para objetos primitivos da composição
||**- Composite:**
||- Define o comportamento para componentes que possuem filhos
||- Armazena componentes filhos
||- Implementa operações relacionadas a filhos e definidas na interface Component
||**- Client:**
||- Manipula os objetos da composição via interface Component
|:heavy_check_mark: **Sample Code**                     |[Links](https://github.com/PF-Henrique/Programacao-Avancada/tree/master/Composite)|
</div>

---

## :movie_camera: **Arquiteture**

<p align="center"><b> :computer: Arquiteture Composite </b>

<p align="center">
  <kbd><img alt="Dino Game" src="https://github.com/PF-Henrique/Programacao-Avancada/blob/master/.docs/composite.jpg"/></kbd>
<p>

---

 # Padrão Template Method

## :memo: **Roteiro**

<div align="center">

|     :computer: topics                                   |     Description    |
|      :---                                               |      :---         |
| :heavy_check_mark: **Pattern Name and Classification**  | - Método de Template Padrão
||- Padrão Comportamental|
| :heavy_check_mark: **Intent**                           |- Permite que as subclasses façam modificações deste algoritimo sem alterar a estrutura  |
| :heavy_check_mark: **Motivation**                       |- Alterações no algoritmo podem ser feitas de forma genética ou específica em cada componente específico|
| :heavy_check_mark: **Applicability**                    | - Aplicação que possui estrutura hierárquica e um algoritmo que pode ser dividido em etapas.
|| - Dois ou mais componentes diferentes implementam esse algoritmo, possuindo várias semelhanças mas algumas diferenças na implementação de algumas etapas do algoritmo.
|| - Alterações no algoritmo podem ser feitas de forma genérica ou específica e componente específico cada Útil em cenários em que se tem um gerador automático de código|
|:heavy_check_mark:   **Participants**                     |Definir o templateMethod que é responsável por chamar os demais métodos.
||Especificações dos métodos abstratos das etapas de execução
||ApplicationClassOne / ApplicationClassTwo:
||Redefine, quando necessário, algumas etapas do algoritmo especificado em FrameworkClass
|:heavy_check_mark: **Sample Code**                     |[Links](https://github.com/PF-Henrique/Programacao-Avancada/tree/master/TemplateMethod)|
</div>

---

## :movie_camera: **Arquiteture**

<p align="center"><b> :computer: Arquiteture Template method </b>

<p align="center">
  <kbd><img alt="Dino Game" src="https://github.com/PF-Henrique/Programacao-Avancada/blob/master/.docs/Template%2BMethod%2B(estrutura).jpg" width= "500px;" height= "250px;" /></kbd>
<p>

---
 
## ✨ Me

<a href="https:https://github.com/PF-Henrique/">
  <img src="https://avatars1.githubusercontent.com/u/48561196?s=460&u=5b39cdc8c6d447868ca0caac900f1ee7a1793962&v=4" width= "50px;" height= "50px;" alt="Avatar"/>
  <br />
 <sub>
  <b>
    Pedro Ferreira
  </b>
</sub>
</a> 
<a href="<a href="https:https://github.com/PF-Henrique/" title="ProductHunt">🚀:octocat:</a>
<br />
