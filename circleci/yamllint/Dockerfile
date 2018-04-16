FROM alpine:3.7
RUN	apk add --no-cache python2 py2-pip && \
	pip install -q yamllint && \
	apk del --no-cache py2-pip && \
	rm -rf $HOME/.cache

ENTRYPOINT ["yamllint"]
