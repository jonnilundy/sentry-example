FROM sentry:8

CMD '/bin/bash -c sentry upgrade --no-input && /entrypoint.sh run web || /entrypoint.sh run web'
