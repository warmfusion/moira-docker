

## Running

    docker-compose up


## Testing

### UX

Navigate to http://$(docker-machine ip dev):8080/

### Send test data

     while [ true ]; \
     do \
        echo "local.random.diceroll $(expr $(date +%s) % 255) `date +%s`" | nc $(docker-machine ip dev) 2003; \
        sleep 1; \
      done
