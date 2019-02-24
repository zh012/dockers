FROM python:3.7-alpine3.8 as base

FROM base as builder

RUN apk update && apk add build-base
RUN pip install --install-option="--prefix=/install" ujson gevent


FROM base

COPY --from=builder /install /usr/local
