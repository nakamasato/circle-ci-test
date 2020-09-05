# circle-ci-test

## Run in local

```
circleci local execute -c .circleci/config.yml
Docker image digest: sha256:a705e4489616fccc12c07c209f48edb95c1749a69d29dfc7e87bb9fe25553a40
====>> Spin up environment
Build-agent version  ()
Docker Engine Version: 19.03.12
Kernel Version: Linux 3bf753e522c8 4.19.76-linuxkit #1 SMP Tue May 26 11:42:35 UTC 2020 x86_64 Linux
Starting container buildpack-deps:trusty
  
trusty: Pulling from library/buildpack-deps
Digest: sha256:bdafcfdbf9ecc32179bb31b781b4cda388a9dc9455c474a17a06550ab90acacc
Status: Image is up to date for buildpack-deps:trusty
  pull stats: N/A
  time to create container: 62ms
  using image buildpack-deps@sha256:bdafcfdbf9ecc32179bb31b781b4cda388a9dc9455c474a17a06550ab90acacc
Starting container mongo
  
latest: Pulling from library/mongo
Digest: sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
Status: Image is up to date for mongo:latest
  pull stats: N/A
  time to create container: 82ms
  using image mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
Starting container mysql:5.7
  
5.7: Pulling from library/mysql
bf5952930446: Already exists 
8254623a9871: Already exists 
938e3e06dac4: Already exists 
ea28ebf28884: Already exists 
f3cef38785c2: Already exists 
894f9792565a: Already exists 
1d8a57523420: Already exists 
5f09bf1d31c1: Already exists 
1591b28581e8: Pull complete 
96ef942f7603: Pull complete 
2e009731422e: Pull complete 
Digest: sha256:1a83136153b238b659b0887ceb4e08275473af1eab2e67de4c22b37c5f4130cd
Status: Downloaded newer image for mysql:5.7
  pull stats: download 102.8MiB in 25.956s (3.96MiB/s), extract 102.8MiB in 4.494s (22.87MiB/s)
  time to create container: 699ms
  using image mysql@sha256:1a83136153b238b659b0887ceb4e08275473af1eab2e67de4c22b37c5f4130cd
Time to upload agent and config: 851.165377ms
Time to start containers: 949.21598ms
====>> Container mongo
====>> Container mysql:5.7
====>> Preparing environment variables
Using build environment variables:
  BASH_ENV=/tmp/.bash_env-localbuild-1599280693
  CI=true
  CIRCLECI=true
  CIRCLE_BRANCH=multiple-container
  CIRCLE_BUILD_NUM=
  CIRCLE_JOB=build
  CIRCLE_NODE_INDEX=0
  CIRCLE_NODE_TOTAL=1
  CIRCLE_REPOSITORY_URL=git@github.com:nakamasato/circle-ci-test
  CIRCLE_SHA1=d356ddec6f36843ec7af2e14a327f45b2c693230
  CIRCLE_SHELL_ENV=/tmp/.bash_env-localbuild-1599280693
  CIRCLE_WORKING_DIRECTORY=~/


The redacted variables listed above will be masked in run step output.====>> sleep 5
nc -vz localhost 27017
sleep 10
nc -vz localhost 3306

  #!/bin/bash -eo pipefail
sleep 5
nc -vz localhost 27017
sleep 10
nc -vz localhost 3306

Connection to localhost 27017 port [tcp/*] succeeded!
Connection to localhost 3306 port [tcp/mysql] succeeded!
Success!
Step canceled
Step canceled
```
