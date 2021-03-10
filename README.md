# Senac_project
Todos os projetos feitos durante o curso Análise e desenvolvimento de sistemas



console.log('Bem vindo ao Calculador');
do
{
/*Estou usando o While do, então o do foi adcionado antes da parte que deve repetir abrindo com { e fechando }   */

 function promptFloat(mensagem, tenteNovamente) {
    var msg = mensagem; 
    while (true) {
        var ret = parseFloat(prompt(msg));
        if (!isNaN(ret)) return ret;
        msg = tenteNovamente;
    }
};
/* Preciso que apenas números possam ser inseridos, então essa função faz com que ao adcionar outro valor, uma mensagem vai aparecer e pedir para inserir um número   */

var gas = parseFloat( promptFloat("Digite o valor da gasolina", "Por favor, digite um número.\nTente novamente."));

/* Aqui foi definido o nome da variável (gas) que simbolizar o valor da Gasolina */


var alc = parseFloat( promptFloat("Digite o valor do álcool", "Por favor, digite um número.\nTente novamente."));
/* Aqui foi definido o nome da variável (alc) que simbolizar o valor do Álcool */

console.log('________________________________');

var resul = (alc/gas);
/* Aqui sai ocorrerá a divisão dos dois valores inseridos */

var total = resul.toFixed(2);

/* Foi usado o toFixed para adcionar duas casas decimais ao valor e não mostrar o todo do número  */

console.log('A divisão dos valores resultou em: '+ total );


if(total > 0.7) {
  console.log('Abasteça com gasolina')
}
if (total < 0.7) {
  console.log('Abasteça com álcool')
}

 else if  (total == 0.7) {
  console.log('Tanto faz abastecer com álcool ou gasolina')
 }
 
/* Aqui foi declarado as variáveis para a mensagem pós resultado
1a Se o resultado da divisão for < (maior)
que 0,7 ;
2o Se o resultado for > (menor) que 0,7;
3o Se o resultado for ==(igual) a 0,7
*/

console.log ('________________________________')
;


var retry = prompt('Deseja refazer consulta ? Digite S: ');
/* Uma variável que vai estabelecer se ocorrerá a repetição ou fechar o programa */

}
while ( retry == 'S');
/* Usamos aqui o == para que ele compreenda tanto o s como o S */
console.log ('Volte Sempre');
/* Fim do código */









