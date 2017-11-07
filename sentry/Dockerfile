FROM sentry:latest

ENTRYPOINT ["/bin/bash","-c"]

CMD [ "sentry upgrade --noinput && sentry createuser --email $SENTRY_INITIAL_USER_EMAIL --password $SENTRY_INITIAL_USER_PASSWORD --superuser && /entrypoint.sh run web || /entrypoint.sh run web" ]
