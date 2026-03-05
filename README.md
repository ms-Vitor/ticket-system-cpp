🎟️ Sistema Ingresso | Gestão de Ingressos em C++
Este projeto é uma aplicação de linha de comando (CLI) desenvolvida para gerenciar o ciclo de vida de ingressos, desde o cadastro até a busca otimizada. O foco principal foi aplicar na prática conceitos fundamentais de estrutura de dados, algoritmos e manipulação de arquivos.

🛠️ Tecnologias e Ferramentas
Linguagem: C++ (Padrão ISO/IEC 14882)
Armazenamento: Persistência em arquivos CSV via biblioteca fstream.
Paradigma: Programação Estruturada e Modular.

💡 Conceitos de Ciência da Computação Aplicados
Este projeto não é apenas um cadastro, mas um laboratório de conceitos fundamentais:

🃏 Ordenação com Insertion Sort
O que é: Funciona como organizar cartas de baralho na mão: você pega um novo ingresso e o "encaixa" na posição correta entre os que já estão ordenados.

Por que usei: É um método muito eficiente para listas que estão sendo construídas aos poucos, garantindo que os dados estejam sempre em ordem para a busca.

🔍 Busca Binária (Binary Search)
O que é: Em vez de procurar um ingresso um por um (do início ao fim), o sistema olha sempre o item do meio da lista. Se o ID for menor, ele descarta a metade direita; se for maior, descarta a esquerda.

Por que usei: Isso torna a localização de um usuário extremamente veloz. Mesmo com milhares de registros, o sistema encontra o alvo em pouquíssimos passos.

🧠 Gerenciamento de Memória (new e delete)
Alocação Dinâmica: Utilizei os operadores new e delete para que o programa utilize apenas a memória RAM necessária para a quantidade exata de ingressos cadastrados.

Eficiência: O controle manual garante que a memória seja liberada após o uso, evitando desperdícios de recursos do computador (memory leaks).

💾 Persistência de Dados (Arquivos CSV)
O que é: O sistema salva e lê todas as informações cadastradas em um arquivo externo usando a biblioteca fstream.

Por que usei: Para garantir que os dados não "sumam" quando o programa é fechado. Isso cria um histórico permanente em formato .csv, funcionando como um banco de dados simples, leve e organizado.

🏗️ Estrutura das Funções Principais
*insertion(): Mantém a base de dados organizada por ID.

*buscaBinaria(): Localiza informações de forma otimizada.

*salvar_no_arquivo(): Exporta os dados para o formato CSV.

*leitura(): Reconstrói a lista de ingressos a partir do arquivo salvo.

🚀 Como Compilar e Rodar
Certifique-se de ter um compilador (GCC/G++) instalado:

Clone o repositório ou baixe o arquivo .cpp.

Abra o terminal na pasta do arquivo e compile:
➪ g++ cadastro_ingressos.cpp -o sistema_ingressos

Execute o programa:
➪ ./sistema_ingressos
📝 Notas do Autor
Este projeto reflete meu aprendizado em lógica de programação e manipulação de baixo nível em C++. Ele demonstra como decisões técnicas simples (como a escolha de um algoritmo de busca) podem impactar diretamente na performance e usabilidade de um software.
