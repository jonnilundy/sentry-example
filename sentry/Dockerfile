FROM sentry:8.22.0

RUN apt-get update && apt-get install -y --no-install-recommends \
        curl \
&& rm -rf /var/lib/apt/lists/*

ENTRYPOINT ["/bin/bash","-c"]

CMD [ "sentry upgrade --noinput && sentry createuser --email $SENTRY_INITIAL_USER_EMAIL --password $SENTRY_INITIAL_USER_PASSWORD --superuser && /entrypoint.sh run web || /entrypoint.sh run web" ]
