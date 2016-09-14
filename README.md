# dm-share

## what ?

A tool to export and import docker-machine credentials.  
It follows the UNIX philosophy by exploiting command composition, pipes, inputs and outputs.

## export

    export name=my_machine_name
    docker-machine inspect $name | dm-export > $name.json

## import

    cat $name.json | dm-import $name

