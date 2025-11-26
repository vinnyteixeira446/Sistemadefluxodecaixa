class FluxoDeCaixa {
  constructor(saldoInicial = 0) {
    this.saldo = saldoInicial;
    this.movimentacoes = [];
  }

  adicionarEntrada(valor) {
    if (valor > 0) {
      this.movimentacoes.push({ tipo: 'entrada', valor: valor });
      this.saldo += valor;
    } else {
      console.log("Valor de entrada deve ser positivo.");
    }
  }

  adicionarSaida(valor) {
    if (valor > 0) {
      this.movimentacoes.push({ tipo: 'saida', valor: valor });
      this.saldo -= valor;
    } else {
      console.log("Valor de saída deve ser positivo.");
    }
  }

  calcularSaldoAtual() {
    return this.saldo;
  }

  listarMovimentacoes() {
    return this.movimentacoes;
  }
}

// Exemplo de uso:
const caixa = new FluxoDeCaixa(1000); // saldo inicial de 1000
caixa.adicionarEntrada(500);          // adiciona receita de 500
caixa.adicionarSaida(200);            // adiciona despesa de 200
caixa.adicionarEntrada(300);          // adiciona receita de 300

console.log("Saldo atual do fluxo de caixa:", caixa.calcularSaldoAtual());
console.log("Movimentações:", caixa.listarMovimentacoes());
