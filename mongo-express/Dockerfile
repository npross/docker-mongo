FROM mongo-express:latest

COPY env_secrets_expand.sh env_secrets_expand.sh
COPY ./entrypoint.sh entrypoint.sh

ENTRYPOINT ["./entrypoint.sh"]
CMD ["tini", "--", "node", "app"]
