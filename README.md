# User Analytics

[Matomo](https://matomo.org/) is a free and open source web analytics application. Matomo is an alternative to Google Analytics and is designed to be more privacy-focused.

## Setup

Setup is performed using the `docker-compose.yml` file. [This example](https://github.com/matomo-org/docker/tree/master/.examples) is the starting point. Example needs the fix explained [here](https://github.com/matomo-org/docker/issues/230#issuecomment-757365994). 

Docker compose setup is executed as part of the ansible playbook. 

### Configuration

After installation by ansible, further configuration is performed by the user on the matomo web interface.
Additinally, matomo tag manager is used to track user interactions in the react app. [This document](https://matomo.org/faq/new-to-piwik/how-do-i-start-tracking-data-with-matomo-on-websites-that-use-react/) explains how to set up matomo tag manager.
