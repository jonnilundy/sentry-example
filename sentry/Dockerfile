FROM sentry:latest

CMD [ "/bin/bash -c sentry upgrade --no-input && sentry createuser --email $SENTRY_INITIAL_USER_EMAIL --password $SENTRY_INITIAL_USER_PASSWORD --superuser && /entrypoint.sh run web || /entrypoint.sh run web" ]
