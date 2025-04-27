# The Herranz's Public Notebooks

This repo contains some of my livebook notebooks that I have used in Workshops and Talks about Elixir.

 🇪🇸 *Este repo contiene algunos de mis cuadernos de livebooks.*

## Feedback is welcome!

Please, [create an issue](https://github.com/aherranz/public_notebooks/issues/new) if you find erros or simply want to discuss about the content of a notebook.

## Start livebook from docker

Although it is not absolutely needed, I recommend you to clone this
repo and `cd` to the directory.

The following command starts the Livebook webapp in a container mounting the
host working directory in the `/data` directory in the container.

```
docker run -p 8080:8080 -p 8081:8081 --pull always -u $(id -u):$(id -g) -v $(pwd):/data ghcr.io/livebook-dev/livebook:0.14.5
```

Open in a browser the URL where the Livebook server is running at. If
your working directory is a clone of this repo you can *Open* any of
my notebooks (e.g.  the functional programming workshop
`pf_en_elixir.livemd`). If you decided not to clone this repo, you can
*Open* a notebook directly from a URL (e.g. [this functional
programming workshop
URL](https://github.com/aherranz/public_notebooks/blob/main/pf_en_elixir.livemd))
or from any file that you have previously downloaded.

**Security Note:** Livebook has access to any file and can execute any
code so using this command at least we confine the problem to the
container itself and to the host working directory.

## Completed notebooks (*Cuadernos terminados*)

After starting livebook you can open any of theese notebooks:

- 🇪🇸 **Taller de programación funcional**
  ([pf_en_elixir.livemd](pf_en_elixir.livemd)): Cuaderno con un taller
  para acercar la programación funcional a programadores con o sin
  experiencia en la misma. Se tratan los elementos fundamentales de la
  programación funcional: inmutabilidad, recursividad, pattern
  matching y funciones de orden superior.
- 🇪🇸 **¿Pero qué demonios es un GenServer?**
  ([demonios_de_genserver.livemd](demonios_de_genserver.livemd)):
  Cuaderno con una presentación realizada conjuntamente en las
  comunidades de [Madrid
  Elixir](https://www.meetup.com/madrid-elixir/) y
  [Madrid.rb](https://www.madridrb.com/) en el que se desmitifica lo
  que realmente es un
  [GenServer](https://hexdocs.pm/elixir/GenServer.html).
