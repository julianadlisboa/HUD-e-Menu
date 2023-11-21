# HUD-e-Menu
ALUNOS: JULIANA LISBOA E GABRIEL TOLEDO

<H1> projeto HUD/MENU <H1/>

Nosso projeto apresenta um menu principal com opção de iniciar ou sair, ao clicar em  "iniciar" o jogo começa e quando a bolinha toca no alvo o jogo abre um menu de fim de jogo com opção de recomeçar ou sair do jogo.

<H2> imagem do menu principal </H2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/c808387b-cdbd-40b4-bc84-6073cb555485)

<h2>Tela do jogo</h2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/ac0d55c9-f54b-4414-b50a-e140068116d9)

<H2> imagem do menu fim de jogo </H2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/3425458e-3ae8-4039-a227-445454ea39e4)


<h2>Load Game Script:</h2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/bd089ca5-44e6-44a7-b6bc-2272deffff03)

Ambos os métodos são públicos, o que significa que podem ser chamados de fora da classe (por exemplo, por um botão em uma interface de usuário Unity). O método CarregarFase1 carrega uma cena específica, enquanto o método Sair encerra o aplicativo.

<h2>Colission color Script:</h2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/aaf738bb-81e0-4650-8957-86bda154fe9f)

Método OnCollisionEnter(Collision collision):
Este método é chamado quando o objeto associado a esse script colide com outro objeto. Se a colisão ocorre com um objeto chamado "Cube", ele imprime "Enter" no console e muda a cor do material do objeto associado para verde.

Método OnCollisionExit(Collision collision):
Este método é chamado quando a colisão com o objeto chamado "Cube" termina. Ele imprime "Exit" no console e muda a cor do material do objeto associado para azul.

Método OnCollisionStay(Collision collision):
Ele imprime "Stay" no console e rotaciona o objeto colidindo ao longo do eixo Z, aplicando uma rotação de -30 graus por segundo.

Portanto, este script está controlando o comportamento do objeto associado em resposta a colisões com um objeto chamado "Cube", alterando a cor do objeto durante a entrada e a saída da colisão, e realizando uma rotação enquanto permanece em colisão.



<h2>Script botões fim de cena:</h2>

![image](https://github.com/julianadlisboa/HUD-e-Menu/assets/128002239/31aa4985-32a0-42c9-ad50-7552fbe041fd)

Namespaces:
Esses são os namespaces utilizados no script. Eles fornecem acesso a bibliotecas que contêm classes e funcionalidades específicas do C# e do Unity.

Classe CarregarFase1:
Aqui, é declarada uma classe chamada CarregarFase1, que herda da classe MonoBehaviour.

Método Voltar():
Este método é público (public) e não retorna nenhum valor (void). Ele usa a classe SceneManager do Unity para carregar uma cena chamada "Menu". Isso geralmente é usado para implementar a funcionalidade de voltar para o menu principal ou para outra cena do jogo.

Método Reiniciar():
Similar ao método Voltar(), este método carrega uma cena chamada "jogocolisores". Isso geralmente é usado para reiniciar a fase ou recarregar uma cena específica do jogo.

Método Fechar():
Este método usa a classe Application do Unity para encerrar o aplicativo. Isso geralmente é usado para fechar o jogo quando chamado.
