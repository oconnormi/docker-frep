# Dockerized frep

Builds a statically-linked version of [frep](https://github.com/subchen/frep) and creates a docker image

#Usage

```bash
docker run --rm oconnormi/frep
```

Pass templates into `oconnormi/frep` using volumes

```bash
docker run --rm -v $(pwd)/templates:/in -v $(pwd)/out:/out oconnormi/frep /in/<templateName>:/out/<fileName>
```

For more usage info see the [Frep Readme](https://github.com/subchen/frep/blob/master/README.md)
