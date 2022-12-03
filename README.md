# Traefik certs exporter

Script opens `acme.json` file from `input` folder and export it's content to `output` folder as `*.cer` and `*.key` files.

There is template `acme.json` file in `input` directory for demonstration purposes. It is added in `.gitignore` - feel free to modify or delete it.

## Usage

Mount your acme.json to /input/ folder and run script

```bash
go run traefik-certs-exporter.go
```

or just use compiled one from Dockerhub

```bash
docker run -v ${PWD}/input:/input -v ${PWD}/output:/output: docker.io/nett00n/traefik-certs-exporter:1.0.0
```

## Links

- [Gihtub Project](https://github.com/nett00n/traefik-certs-exporter)
- [DockerHub Page](https://hub.docker.com/r/nett00n/traefik-certs-exporter)

## License

All code in this repository is licensed under the terms of the MIT License. For further information please refer to the LICENSE file.

## Authors

- Vladimir Budylnikov aka [@nett00n](https://github.com/nett00n)

---
2022, Yerevan
