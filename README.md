# curloop
Docker Alpine-based image with cURL for cyclic poking some URL

## Usage

```console
$ docker run --rm --link api-prod curloop 10 http://api-prod:3000/method/daemon.run -fsSX POST

$ docker run --rm curloop curl -sSL https://gmail.com"

$ docker run --rm curloop sh -c "while sleep 10; do curl -s www.ru || echo err; done"
```

## Environment variables

* `LOOP_CURL` 
* `LOOP_SECS`

## License

Copyright (c) 2018 Anton A. Pukhov

All contents licensed under the [MIT License](LICENSE)
