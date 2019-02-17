# codebuild-logs
Gets logs for most recent run of a codebuild project.

## Usage
To list all codebuild projects in your default region:
```shell
codebuild-logs
```

A different AWS profile and another region can both be optionally specified, e.g.
```shell
codebuild-logs --region ap-southeast-2
```
lists all codebuild projects in the ap-southeast-2 (Sydney) region and
```shell
codebuild-logs --profile myprofile --region ap-southeast-2
```
also specifies that the profile `myprofile` is used. Refer to https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-configure.html for more ways to specify credentials and region.

To list the latest codebuild logs for particular project(s) list those as command line parameters, e.g.:
```
codebuild tba21-helpers tba21-api-dev
```
