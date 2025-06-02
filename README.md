# Build/Push Docker GCP Artifact Registry Action

### Summary

This action's job is to build a Docker image, and then push it to GCP's Artifact Registry. It also has chacing enabled, and caches files in GitHub Actions.

### Inputs

##### gcp_credentials_json

- This is the GCP Credentials JSON. It is recommended to store the value feeding this input in GitHub secrets.

##### dockerfile_path

- This is the path to the Dockerfile.

##### docker_target

- This is the specified Docker target for Docker build command.

##### tags

- This is the full image name/tag to give Docker image.

##### build_args

- Key-value pairs that will be exported in docker build-args command.

##### workload_identity_provider

- This is the Workload Identity Provider for Google Cloud.

##### service_account

- This is the Service Account for Google Cloud, used with Workload Identity.

##### enable_cache

- This is the enable_cache for Docker build caching.
