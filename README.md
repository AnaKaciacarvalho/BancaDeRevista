# BancaDeRevista
#include <stdio.h>
#include <stdlib.h>

struct Cliente{
    char nome[100];
    char endereco[100];
    int telCliente;
    char cpf[20];
};
struct Revista{
    char nomeRevista[100];
    float preco;
    int ano;
};
struct Fornecedor{
    char nomeFornecedor[100];
    char enderecoFornecedor[100];
    int numeroFornecedor;
    char CNPJ[30];
};
struct Estoque{
    char fornecedor[100];
    int quantidadeEstoque;
    float precoTotal;
};
struct Venda{
    Cliente cliente[100];
    Revista revista[100];
    float preco;
    char vendedor[100];

};


void cadastroCliente(){

    struct Cliente cliente;

    system("cls");

    printf("Digite nome do cliente: ");
    fflush(stdin);
    gets(cliente.nome);

    printf("Digite endereco do cliente: ");
    fflush(stdin);
    gets(cliente.endereco);

    printf("Digite nome do cliente: ");
    fflush(stdin);
    scanf("%d", &cliente.telCliente);

    printf("Digite CPF do cliente: ");
    fflush(stdin);
    gets(cliente.cpf);

}
void cadastroRevista(){}
void cadastrarEstoque(){}
void cadastrarFuncionario(){}
void cadastroVenda(){}

int main()
{
    int op;

    while(1){
        system("cls");
        printf("1) Cadastrar Cliente\n2) Cadastrar Revista\n3) Cadastrar Estoque\n4) Cadastrar Funcionario\n5) Cadastrar Venda\n\nDigite uma opcao: ");
        switch(op){
        case 1:
            cadastroCliente();
        break;
        case 2:
            cadastroRevista()
        break;
        case 3:
            cadastrarFuncionario()
        break;
        case 4:
            cadastroVenda()
        break;
        }
    }

    return 0;
}
