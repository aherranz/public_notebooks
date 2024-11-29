# The Herranz's Public Notebooks

This repo contains some of my livebook notebooks that I have used in Workshops and Talks about Elixir.

 🇪🇸 *Este repo contiene algunos de mis cuadernos de livebooks.*


## Start livebook from docker

This command starts Livebook, a webserver, in a container mounting the
host working directory in the `/data` directory in the container.

```
docker run -p 8080:8080 -p 8081:8081 --pull always -u $(id -u):$(id -g) -v $(pwd):/data ghcr.io/livebook-dev/livebook:0.14.5
```

Using Livebook is easy, once started copy and paste in the browser the
URL from the command in the browser, and open up any of the notebooks
(you can download and open the lifes or you can open any of them
copying the URL).

**Security Note:** Livebook has access to any file and can execute any
code so using this command at least we confine the problem to the
container itself and to the host working directory.

## Completed notebooks (*Cuadernos terminados*)

After starting livebook you can open any of theese notebooks:

- 🇪🇸 [pf_en_elixir.livemd](pf_en_elixir.livemd): Cuaderno con un
  taller para acercar la programación funcional a programadores con o
  sin experiencia en la misma. Se tratan los elementos fundamentales
  de la programación funcional: inmutabilidad, recursividad, pattern
  matching y funciones de orden superior.
