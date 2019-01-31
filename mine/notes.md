docker-compose -f mine/1so2.yaml up -d


docker volume create so1-var
so1-etc
so1-var

volumes:
      - /Volumes/8tb/mounts/docker/splunk/so1-etc:/var/lib/backup/data

volumes:
  data-volume:

  volumes:
      - ./web-app/application:/application