# circle-ci-test

## Run in local

```
circleci local execute -c .circleci/config.yml   Docker image digest: sha256:a705e4489616fccc12c07c209f48edb95c1749a69d29dfc7e87bb9fe25553a40
====>> Spin up environment
Build-agent version  ()
Docker Engine Version: 19.03.12
Kernel Version: Linux 09323c91ddde 4.19.76-linuxkit #1 SMP Tue May 26 11:42:35 UTC 2020 x86_64 Linux
Starting container buildpack-deps:trusty
  
trusty: Pulling from library/buildpack-deps
Digest: sha256:bdafcfdbf9ecc32179bb31b781b4cda388a9dc9455c474a17a06550ab90acacc
Status: Image is up to date for buildpack-deps:trusty
  pull stats: N/A
  time to create container: 86ms
  using image buildpack-deps@sha256:bdafcfdbf9ecc32179bb31b781b4cda388a9dc9455c474a17a06550ab90acacc
Starting container mongo
  
latest: Pulling from library/mongo
Digest: sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
Status: Image is up to date for mongo:latest
  pull stats: N/A
  time to create container: 82ms
  using image mongo@sha256:df9eca84736a666d5f7e7a09aeb8a6d8d073698d5b7349400f10ee75812e0e95
Time to upload agent and config: 925.589286ms
Time to start containers: 681.419214ms
====>> Container mongo
====>> Preparing environment variables
Using build environment variables:
  BASH_ENV=/tmp/.bash_env-localbuild-1599279977
  CI=true
  CIRCLECI=true
  CIRCLE_BRANCH=multiple-container
  CIRCLE_BUILD_NUM=
  CIRCLE_JOB=build
  CIRCLE_NODE_INDEX=0
  CIRCLE_NODE_TOTAL=1
  CIRCLE_REPOSITORY_URL=git@github.com:nakamasato/circle-ci-test
  CIRCLE_SHA1=ee92bae356c1525b8cfb9f937180fadaa9663e35
  CIRCLE_SHELL_ENV=/tmp/.bash_env-localbuild-1599279977
  CIRCLE_WORKING_DIRECTORY=~/


The redacted variables listed above will be masked in run step output.====>> sleep 5 && nc -vz localhost 27017
  #!/bin/bash -eo pipefail
sleep 5 && nc -vz localhost 27017
Connection to localhost 27017 port [tcp/*] succeeded!
Success!
Step canceled
```
