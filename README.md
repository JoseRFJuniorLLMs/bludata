API REST na linguagem Go que faça a gravação de uma câmera conectada ao servidor, com as seguintes 3 rotas, segue descrição:

POST /api/v1/record/start
Parâmetros: nenhum
Retorno:
Status: 200
Body: Gravação iniciada com sucesso
POST /api/v1/record/stop
Parâmetros: nenhum
Retorno:
Status: 200
Body: Gravação finalizada com sucesso
GET /api/v1/record
Parâmetros: nenhum
Retorno: Download do arquivo gravado
Observações: A API deve rodar em ambiente Linux

## capture
---

just some golang with some opencv, and a fun-project playing around with your webcam

---

### Requirements:

This project's main dependencies are OpenCV and Golang as distro level packages. These users/developers need to install themselves.

Then in golang it depends on [lazywei/go-opencv](github.com/lazywei/go-opencv/opencv) golang package to use OpenCV system API.
This (and any other future dependency) can be managed by running

```bash
./go-tasks.sh deps
```

---

### Build

Building this to a binary requires installing all dependencies and then using go-build.
Following command helps in isntalling all golang-package dependencies and creating binary in a go...

```bash
./go-tasks.sh bin
```

The binaries are placed in {PROJECT-PATH}/bin

---

### Running

Once build, it can be run by executing binaries from the stated binary paths in Build section.

To do all in one show, run...

```bash
./go-tasks.sh run
```

---

# bludata
