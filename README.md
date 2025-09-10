# **combobox-java-frame-nebeans**
Código em java, ambientado em NetBeans descrevendo alguns dos funcionamentos da caixa de combinação

## **Detalhas sobre a combobox:**
Em Java, um componente JComboBox (caixa de combinação) é um elemento gráfico de interface do utilizador (GUI) da biblioteca Swing que combina um campo de texto editável e uma lista suspensa para que o utilizador possa selecionar um item de uma lista ou inserir um valor personalizado. 

## **Tabela jcombobox:**

| **Categoria**            | **Método**                             | **Descrição**                                        | **Exemplo de uso**                                                                                                     |
| ------------------------ | -------------------------------------- | ---------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------- |
| **Manipulação de Itens** | `addItem(Object item)`                 | Adiciona um item ao final da lista.                  | `cbCores.addItem("Azul");`                                                                                             |
|                          | `insertItemAt(Object item, int index)` | Insere um item em uma posição específica.            | `cbCores.insertItemAt("Verde", 1);`                                                                                    |
|                          | `removeItem(Object item)`              | Remove a primeira ocorrência do item informado.      | `cbCores.removeItem("Azul");`                                                                                          |
|                          | `removeItemAt(int index)`              | Remove o item pelo índice.                           | `cbCores.removeItemAt(0);`                                                                                             |
|                          | `removeAllItems()`                     | Remove todos os itens do `JComboBox`.                | `cbCores.removeAllItems();`                                                                                            |
| **Seleção de Itens**     | `getSelectedItem()`                    | Retorna o item selecionado (objeto).                 | `Object cor = cbCores.getSelectedItem();`                                                                              |
|                          | `setSelectedItem(Object item)`         | Seleciona o item informado (se existir).             | `cbCores.setSelectedItem("Vermelho");`                                                                                 |
|                          | `getSelectedIndex()`                   | Retorna o índice do item selecionado.                | `int i = cbCores.getSelectedIndex();`                                                                                  |
|                          | `setSelectedIndex(int index)`          | Seleciona o item pelo índice.                        | `cbCores.setSelectedIndex(2);`                                                                                         |
| **Informações**          | `getItemAt(int index)`                 | Retorna o item em determinada posição.               | `String cor = (String) cbCores.getItemAt(1);`                                                                          |
|                          | `getItemCount()`                       | Retorna o número total de itens.                     | `int qtd = cbCores.getItemCount();`                                                                                    |
| **Aparência**            | `setEditable(boolean editable)`        | Define se o usuário pode digitar valores.            | `cbCores.setEditable(true);`                                                                                           |
|                          | `isEditable()`                         | Retorna se o combo é editável.                       | `boolean edit = cbCores.isEditable();`                                                                                 |
|                          | `setEnabled(boolean enabled)`          | Ativa/desativa o `JComboBox`.                        | `cbCores.setEnabled(false);`                                                                                           |
|                          | `isEnabled()`                          | Verifica se está ativo.                              | `boolean ativo = cbCores.isEnabled();`                                                                                 |
|                          | `setBackground(Color c)`               | Define a cor de fundo.                               | `cbCores.setBackground(Color.LIGHT_GRAY);`                                                                             |
|                          | `setForeground(Color c)`               | Define a cor do texto.                               | `cbCores.setForeground(Color.BLUE);`                                                                                   |
|                          | `setFont(Font f)`                      | Define a fonte.                                      | `cbCores.setFont(new Font("Arial", Font.BOLD, 14));`                                                                   |
| **Eventos**              | `addActionListener(ActionListener l)`  | Executa ação quando há seleção no combo.             | `java cbCores.addActionListener(e -> { System.out.println(cbCores.getSelectedItem()); });`                             |
|                          | `addItemListener(ItemListener l)`      | Detecta quando item é selecionado ou desselecionado. | `java cbCores.addItemListener(e -> { if (e.getStateChange()==ItemEvent.SELECTED) System.out.println(e.getItem()); });` |
