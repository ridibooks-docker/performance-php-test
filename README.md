Docker image for CI tests
========================================================

[![](https://images.microbadger.com/badges/version/ridibooks/performance-php-test.svg)](http://microbadger.com/images/ridibooks/performance-php-test "Get your own version badge on microbadger.com")
[![](https://images.microbadger.com/badges/image/ridibooks/performance-php-test.svg)](http://microbadger.com/images/ridibooks/performance-php-test "Get your own version badge on microbadger.com")
[![Build Status](https://travis-ci.org/ridibooks-docker/performance-php-test.svg?branch=master)](https://travis-ci.org/ridibooks-docker/performance-php-test)

Test with Gitlab Runner
-----
1. Write `.gitlab-ci.yml` using this image in your project.
2. To run ci task in local machine, install [gitlab-ci-multi-runner](https://gitlab.com/gitlab-org/gitlab-ci-multi-runner)
3. Run gitlab-ci-multi-runner in the project dir:

```
# without SSH key
gitlab-runner exec docker [task_name]

# with SSH key
gitlab-runner exec docker [task_name] --env SSH_PRIVATE_KEY="`cat ~/.ssh/id_rsa`"
```
