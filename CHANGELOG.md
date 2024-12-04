# Change Log
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/) and this project adheres to 
[Semantic Versioning](http://semver.org/).

## 4.0.0

### Added minimal python3 dependency for managed nodes

- managed nodes require python version of at least 3.5 (
  see: https://docs.ansible.com/ansible/2.9/dev_guide/developing_python_3.html#minimum-version-of-python-3-x-and-python-2-x
  and https://docs.ansible.com/ansible/latest/reference_appendices/release_and_maintenance.html#ansible-core-support-matrix)

## 3.0.0

### Added

- use `community.crypto.x509_certificate_info` instead of `openssl_certificate`,
  As of Ansible 2.10, the 'openssl_certificate' was moved to the 'community.crypto'
  collection and the 'assertonly' provider was removed.

## 2.3.0

### Added

- support lego's `--preferred-chain` flag to be able to remove legacy expired certs from the chain.

## 2.2.0

### Added

- allow injecting env vars for custom service authentication, e.g. CloudFlare.

## 2.1.0

### Added

- install let's encrypt CA as trusted

## 2.0.0

### Added

- remove existing cert if it is not valid, e.g. snakeoil cert

## 1.1.0

### Added

- silence cron jobs

## 1.0.0

### Added

- Everything. This is the initial release.
