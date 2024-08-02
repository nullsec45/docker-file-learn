FROM alpine:3

LABEL autbor="Rama Fajar Fadhillah"
LABEL company="STT Terpadu Nurul Fikri"
LABEL instagram="@fajar.php"


RUN mkdir hello
RUN echo "Hello World" > "hello/world.txt"
ADD text/*.txt hello

CMD cat "hello/world.txt"

