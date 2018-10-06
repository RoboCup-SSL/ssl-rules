# RoboCup Small Size League rules

This is the AsciiDoc source for the official RoboCup Small Size League rules.
The legacy version of the rules can be found at https://github.com/RoboCup-SSL/ssl-rules-legacy

## Build
The rules are automatically built on updates to the master branch and published to [Github Pages](https://robocup-ssl.github.io/ssl-rules/sslrules.html). There is also a [PDF-version](https://robocup-ssl.github.io/ssl-rules/sslrules.pdf).

### Using AsciiDoctor natively
Install AsciiDoctor on your system (https://asciidoctor.org/). Afterwards, build HTML5 version with
```
# Build the HTML5 version
asciidoctor sslrules.adoc
# Build the PDF version
asciidoctor-pdf sslrules.adoc
```

### Using docker image
If you have Docker installed, you can use the official AsciiDoctor image:
```
# Pull image once
docker pull asciidoctor/docker-asciidoctor
# Build the HTML5 version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor sslrules.adoc
# Build the PDF version
docker run -v $PWD:/documents/ asciidoctor/docker-asciidoctor asciidoctor-pdf sslrules.adoc
```
