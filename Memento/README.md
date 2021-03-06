# **Markdown**

## 1. **Pattern Name and Classification:**
* Padrão Memento
* Padrão Comportamental

## 2. **Intent:**
*  Permite capturar e externalizar um estado interno de um objeto, de maneira que o objeto possa ser restaurado para esse estado mais tarde, sem violar o encapsulamento.

## 3. **Motivition:**
* Quando houver necessidade de registrar o estado interno de um objeto para implementação 
  de mecanismo de checkpoints e para desfazer operações no caso de erro

* Porém, objetos normalmente encapsulam parte ou todos os seus estados, tornando-os inacessíveis a outros objetos e impossíveis de serem salvos externamente. Expor este estado violaria o encapsulamento, o que pode comprometer a confiabilidade e a extensibilidade da aplicação.

* O objetivo do padrão é fornecer um mecanismo para permitir atender esta demanda sem violar o princípio de encapsulamento da Orientação a Objetos.

## 4. **Applicability:**
* Sempre quando houver a necessidade de se criar pontos de restauração de estado de objetos.

* Permitir que o programa se recupere de erros.

## 5. **Structure:**

<p align="center">
  <img alt="Wyden" src="https://github.com/PF-Henrique/Programacao-Avancada/blob/master/.docs/Memento.png" />
<p>


## 6. **Participants:**

######    **Memento:**
* classe que representa um snapshot, contendo o estado de um objeto a ser restaurado em um Originador. Possui métodos para obter e definir o estado que um Memento encapsula dentro

######    **Originador:**
* classe na qual o estado atual é mantido. Define método que permite criar um Memento com o estado atual do Originador armazenado no Memento retornado. Originator também tem um método que define seu estado atual com o estado de um determinado objeto Memento. Portanto, pode criar um Snapshot  (Memento) ou restaurar o estado do Snapshot fornecido (Memento).   

######    **Caretaker:**
* classe auxiliar responsável por armazenar e restaurar o estado do Originador por meio do objeto Memento. Um objeto Caretaker mantém os Mementos, mas nunca modifica os Mementos. 


## 7. **Sample Code:**
1. [memento repl.it](https://repl.it/@JoaoRonaldo/MementoPatternDotNet-1)
* Neste código possui uma interface que permite escrever um texto, desfazer a operação de escrita e exibir o texto no terminal. Ao escrever um novo texto, primeiro o estado é salvo, então a alteração é feita. Ao desfazer a escrita é solicitado ao Caretaker que pegue o último estado salvo, a partir deste estado é possível pegar o texto e restaurá-lo.


