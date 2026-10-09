# python6.
entregael de pytho da semana 6
class Produto:

    def __init__(self, nome, preco):
        self.nome = nome
        self.preco = preco

    def __str__(self):
        return f"{self.nome} - R$ {self.preco}"


class Livro(Produto):

    def __init__(self, nome, preco, autor):
        super().__init__(nome, preco)
        self.autor = autor

    def __str__(self):
        return f"Livro: {self.nome} ({self.autor}) - R$ {self.preco}"


class Eletronico(Produto):

    def __init__(self, nome, preco, voltagem):
        super().__init__(nome, preco)
        self.voltagem = voltagem

    def __str__(self):
        return f"Eletrônico: {self.nome} ({self.voltagem}V) - R$ {self.preco}"


p1 = Produto("Cadeira", 350.0)
p2 = Livro("Entendendo Algoritmos", 59.9, "Aditya Bhargava")
p3 = Eletronico("Teclado Gamer", 220.0, 110)

print(p1)
print(p2)
print(p3)
