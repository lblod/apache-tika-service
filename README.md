# apache-tika-service
Extended version of Apache Tika with tesseract-ocr-nld

# How to use

## Docker-compose

Add the following snippet in your `docker-compose.yml`:

```
  apache-tika:
    image: lblod/apache-tika-service
```

In your `docker-compose.override.yml`, you can test the endpoint:

```
apache-tika:
  ports:
    - "9998:9998"
```

## In code

An example of sending a PDF to the service can be found in the `extract_content_from_pdf` function of the [pdf-content-extraction-service](https://github.com/semantic-ai/decide-pdf-content-extraction).
