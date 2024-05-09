# jogo-secreto-
// as pessoas rem que adivinhar qual é o número secreto 

alert('Boas vindas ao jogo do número secreto');
let numeroSecreto = 4;
console.log(numeroSecreto)
let chute;
let tentativas = 1;

// enquanto chute não for igual ao n.s.
while (chute != numeroSecreto) {
    chute = prompt('escolha um número entre 1 e 10');
    //se chute for igual ao número secreto
    if (chute == numeroSecreto) {
       alert(`isso ai! você descobriu o numero secreto ${numeroSecreto} com ${tentativas} tentativas`);
    } else {
        if (chute > numeroSecreto) {
            alert(`o numero secreto é menor que ${chute}`);
        } else {
            alert(`o numero secreto é maior que ${chute}`);
        }
       // rentativas = tentativas +1;
        tentativas++;
    }
}
