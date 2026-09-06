# Aviso

Deixando claro: o texto abaixo partiu de um curso gratuito e não pode ser redistribuído. Se o tema interessar, procure o curso aberto da trilha de Java com Spring Boot. Caso a plataforma retire o acesso ou passe a cobrar, não depende de mim — mas o material é de ótima qualidade e quem assina um plano aproveita bem mais.

O enunciado do desafio está publicado na plataforma do curso, e existe um repositório público com a implementação de referência.

Como já havia feito tudo o que os vídeos mostram, vou explicar os conceitos e onde cada um aparece:

# Abstração

Para modelar uma classe como a de desenvolvedor, é preciso abstrair. No mundo real um desenvolvedor é uma pessoa completa, mas o sistema só se interessa por algumas características e ignora o resto. Uma pessoa come, por exemplo, mas isso não importa aqui. O que importa é que um desenvolvedor consiga progredir num programa de estudos.

# Encapsulamento

Na classe de curso, por exemplo, a carga horária não fica exposta: o valor é lido e alterado por métodos próprios.

# Herança

As classes de curso e de mentoria herdam de uma classe de conteúdo.

# Polimorfismo

Um exemplo é o método que recebe um conjunto de conteúdos na classe de desenvolvedor:

```
    public void setConteudosInscritos(Set<Conteudo> conteudosInscritos) {
        this.conteudosInscritos = conteudosInscritos;
    }
```

A classe de conteúdo é abstrata e genérica, e as de curso e mentoria herdam dela. Como se quer aceitar curso ou mentoria no conjunto, declara-se o tipo da classe base dentro dos genéricos. Isso é polimorfismo.

### Lembrete

Este trecho foi anotado durante os estudos e nao substitui a documentacao oficial.