FROM        debian:testing-slim

ENV REFRESHED_AT 2020-10-12

RUN apt-get update && apt-get upgrade -y  && apt-get install -y --no-install-recommends \
        pandoc

CMD ["pandoc", "/docs/doc.docx", "-f", "docx", "-t", "markdown", "-o", "/docs/doc.md"]

