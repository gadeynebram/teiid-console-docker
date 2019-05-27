# Teiid Docker image With Console

This is an example Dockerfile with [Teiid Runtime engine on Wildfly](http://teiid.io/).

It also includes Teiid Web Console.

## Usage

    docker run -it gadeynebram/teiid-console-docker

## To boot in domain mode:

    docker run -it gadeynebram/teiid-console-docker /opt/jboss/wildfly/bin/domain.sh -b 0.0.0.0 -bmanagement 0.0.0.0

## Extending the image

    FROM gadeynebram/teiid-console-docker
    # Do your stuff here

## Application deployment

With the Teiid server you can deploy your application in multiple ways:

- You can use CLI
- You can use the web console
- You can use the management API directly
- You can use the deployment scanner

## Example
https://developer.jboss.org/wiki/QuickstartExampleWithDockerizedTeiid
