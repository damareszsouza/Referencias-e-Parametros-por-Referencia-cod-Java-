# Referencias-e-Parametros-por-Referencia-cod-Java-

Ir para o conteúdo principal
Damares Costa de Souza 
Moodle - IFRS

Programação Básica com Java III - Turma 2022B
Painel Meus cursos  PBJIII2022B 4. Procedimentos, Funções e Métodos  4.9. Referências e Parâmetros por Referência
4.9. Referências e Parâmetros por Referência
Duas maneiras de passar parâmetros para métodos em muitas linguagens de programação são a passagem por valor e a passagem por referência. A passagem por valor é a que vimos até agora, quando se faz uma cópia do valor do parâmetro e passa-se para o método. Alterações na cópia feitas pelo método chamado não afetam o valor da variável original no código chamador. Por exemplo, considere o método abaixo:

    static void proc(int y) {
            y++;
            System.out.printf(“Durante Y = %d\n”, y);
    }

O parâmetro y, passado para o método proc, é passado por valor. Isso significa que alterações no valor de y não serão propagadas para fora do método. Veja que y é alterado dentro do método. Um exemplo de utilização do método acima é mostrado abaixo. A saída do código é mostrada logo a seguir. Note que o valor da variável x não é alterado pelo método proc. O parâmetro y recebe uma cópia do valor da variável x.

         int x = 1;
         System.out.printf(“Antes X = %d\n”, x);
         proc(x);
         System.out.printf(“Depois X = %d\n”, x);
Imagem mostra o seguinte texto: Antes X = 1 Durante Y = 2 Depois X = 1

Quando um parâmetro é passado por referência, o código chamador dá ao método a capacidade de acessar diretamente os dados de suas variáveis e modificar esses dados se o método chamado assim o escolher. A passagem por referência melhora o desempenho para a passagem de quantidades grandes de dados, porque ela elimina a necessidade de se construir uma cópia dos dados.

Diferentemente de outras linguagens, Java não permite que o programador escolha entre passar cada parâmetro por valor ou por referência. As variáveis dos tipos de dados primitivos sempre são passadas por valor. Variáveis que armazenam vetores ou matrizes são sempre passadas por referência. Veremos um exemplo de passagem por referência na próxima seção.

Passar arranjos por referência faz sentido por razões de desempenho. Se os arranjos fossem passados por valor, uma cópia de cada elemento seria passada. Para os arranjos grandes passados com frequência, isso desperdiçaria tempo e consumiria considerável capacidade de armazenamento para as cópias dos dados.

Última atualização: domingo, 1 nov 2020, 20:48
Seguir para...
Academi
Dúvidas? 
Perguntas frequentes

Fale conosco | Suporte | Contato

Informação
Termos e Condições de Uso
Aviso de Privacidade e Proteção de Dados Pessoais
Contato
Rua Gen. Osório, 348, Bento Gonçalves/RS
Siga-nos
Copyright © 2017 - Desenvolvido por LMSACE.com. Distribuído por Moodle
