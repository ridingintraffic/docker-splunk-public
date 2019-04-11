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


    volumes:
      - type: volume
        source: so1-etc
        target: /nfs
        volume:
          nocopy: true
volumes:
  so1-etc:
    driver_opts:
      type: "nfs"
      o: "addr=192.168.1.123,nolock,soft,rw"
      device: ":/volumeUSB1/usbshare/mounts/docker/splunk/so1-etc"