# status
> Status: Twitter Analytics Tool for User Statistics.

Status is an visualisation tool for an individual's Twitter timeline. It is able
to visualise *events* that occur in relation to the signed in Twitter user, 
e.g., new follower, retweets, etc. It is also able to import statistics 
exported from the Twitter analytics site.

Status consists of two separate components; 1) the Stream component which is 
responsible for monitoring the users' Twitter timelines, and; 2) the Display
component which is responsible for visualising the users' timelines.

## Installation

Status is configured to run as a [Docker Compose](https://docs.docker.com/compose/)
application. You will need to have Docker Compose and [Docker](https://www.docker.com)
installed. Also ensure that you have checked out the `status-stream` and 
`status-display` submodules. Copy the `docker-compose.yml.example`
file to `docker-compose.yml` and edit. You will need a 
[Twitter OAuth key](https://apps.twitter.com/) and a
[Google Maps API key](https://console.developers.google.com/apis). It is
also recommended that you also change some of the other defaults for security.
Once configured, you can run the application with `docker-compose up`. The
web interface will be available on your configured IP and Port.

## Development setup

Ensure first that you have checked out the `status-stream` and 
`status-display` submodules. We use [Vagrant](https://www.vagrantup.com/)
for development, to start copy `vagrant-config.rb.example` to 
`vagrant-config.rb` and edit the contents, each configuration parameter is
documented in the file. Once saved, you can run `vagrant up` to launch
the virtual machine. The development install will be available in a browser at
the IP address you configured.

## Meta

Distributed under the Affero GPLv3 license. See `LICENSE` for more information.

<https://github.com/CREATe-centre/status>
