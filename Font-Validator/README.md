Font-Validator
==============

Dockerfile for [Font-Validator](https://github.com/HinTak/Font-Validator)

Build:

    docker build -t fontvalidator .

Run:

    docker run --rm -it -v /etc/localtime:/etc/localtime:ro -v /home/wmoore/Work/prince-rust/subset.otf:/font.otf:ro -v $(pwd)/out:/out fontvalidator -file /font.otf -report-dir /out
