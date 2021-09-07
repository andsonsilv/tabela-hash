# Tabela-Hash
[hash] Implementação de tabela hash com encadeamento exterior + template

Implementação de uma tabela hash com encadeamento exterior.
Não foi implementado o vetor de listas encadeadas do zero, já que a tabela usa como array o contêiner std::vector do C++.
Cada elemento desse std::vector é um objeto do tipo std::list.

É armazenado na tabela não apenas as chaves, mas também os valores associados a cada chave, cada elemento da lista deve ter a capacidade de armazenar um tipo de dado composto (chave,valor).
Como tipo de dado composto, foi usado o tipo de dado std::pair do C++. Ou seja, cada elemento da std::list será um objeto do tipo std::pair.

Deste modo, a definição que concretiza a noção de tabela hash com encadeamento exterior pode ser feita da seguinte forma:
vector<list<pair<Tkey,Tval>>> table;
Nesta definição, Tkey e Tval são, respectivamente, o tipo da chave e o tipo do valor associado à chave. Esses tipos são tipos genéricos declarados no template de classe HashTable.

Testes encontram-se na pasta 'testes'.

