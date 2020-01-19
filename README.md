# Simple Node.js webserver running Fastify (customized for Elastic Beanstalk)

**Original repository is at [https://github.com/mikaelvesavuori/node-simple-webserver](https://github.com/mikaelvesavuori/node-simple-webserver)**

This package sets up a Fastify server responding to two paths:

- `/` (root), serving a rudimentary HTML page
- `/hello` serving a JSON object with the key `hello` and the value `world`

I made the original version as a basic "go-to" application for the course "Cloud Developer Basics" that I am running.

## Adaptations that you may need to do in Elastic Beanstalk

You may need to customize a few environment parameters in Elastic Beanstalk:

- Set PORT to 8081
- Set startup Node command to `node server.js`
- Remove proxy (default is probably `Nginx`, set to `None`)
