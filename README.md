# Automatos_LFA

Neste notebook temos uma implementação da estrutra de um autômato.

Um automato pode ser criado da seguinte forma:

Cada estado deve ser criado com as seguintes informações:
- Identificador;
- Transições;
- eh_inicial, boolean que define se ele é o estado inicial ou não(Opcional, False como padrão);
- eh_final, boolean que define se ele é um estado final ou não(Opcional, False como padrão).
Ex: q0 = Estado('q0',{'0':'q1','1':'q2'},eh_inicial=True,eh_final=False)

Com todos os estados criados, os estados devem ser colocados em um dict.
Ex: estados = {'q0':q0,'q1':q1,'q2':q2,'q3':q3,'q4':q4}

Por fim, o autômato pode ser criado utilizando a classe AFD:

O construtor de AFD precisa receber os seguintes parâmetros:
- Um dicionário com todos os seus estados;
- O estado inicial;
- Uma list representando o alfabeto para o autômato
Ex: afd = AFD(estados,q0,['0','1'])

Um valor pode ser testado nesse autômato chamando o método entrada:
Ex: qFinal = afd.entrada('01101101')
No qual ele imprime se a entrada foi aceita ou não e retorna o último estado.

Um outro método que pode ser chamado nessa estrutura de autômato é o estados_equivalentes(),
que retorna todos os estados equivalentes e os não equivalentes.
Ex: afd.estados_equivalentes()

Autores:
Leonardo Machado Leite
Ana Carla Gomes da Silva
