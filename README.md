# The Herranz's Public Notebooks

This repo contains some of my livebook notebooks that I have used in Workshops and Talks about Elixir.

 🇪🇸 *Este repo contiene algunos de mis cuadernos de livebooks.*

## Start livebook from docker

This command starts a container mounting the host working directory in
the `/data` directory in the container.  Remember that livebook
has access to any file and can execute any code so using this command
at least we confine the problem to the container itself and the
host working directory.

```
docker run -p 8080:8080 -p 8081:8081 --pull always -u $(id -u):$(id -g) -v $(pwd):/data ghcr.io/livebook-dev/livebook
```

## Completed notebooks (*Cuadernos terminados*)

- 🇪🇸 [pf_en_elixir.livemd](pf_en_elixir.livemd): Cuaderno con un
  taller para acercar la programación funcional a programadores con o
  sin experiencia en la misma. Se tratan los elementos fundamentales
  de la programación funcional: inmutabilidad, recursividad, pattern
  matching y funciones de orden superior.
