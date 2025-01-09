# Running winget.pro

This directory contains files for running winget.pro in various environments:

 * [`local/`](local) contains files for running on your own PC. The instructions
   there are typically followed during development.
 * [`docker/`](docker) lets you run winget.pro via Docker. This has the benefit
   that it works in all environments where Docker is available.
 * [`aspire/`](aspire) runs winget.pro via docker without the use of docker-compose.
   This is useful for environments where docker-compose is not available 
    and allows for multiple deployment strategies and cloud orchestration with out apps.
 * [`vps/`](vps) runs winget.pro on a single Linux VPS. This imposes stricter
   requirements on the environment (namely, that it is a stock Debian server
   without any customizations). But it has the advantage that all that's
   required to do maintenance is to SSH into the server.