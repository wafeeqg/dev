
## ImagePullBackOff
This is very common error and happens when newly created POD's container is failed to fetch the image from the container registry. It may happen due to following reasons;
- network error
- image name, tag is wrong or does not exist
- wrong credentials (insufficient permissions) to pull an image from the image repository.

When this error occurs, the POD will remain in the Pending State and it needs to be resolved. It can be troubleshooted by commands like `describe` etc.
- if the name or tag is wrong, it can be corrected and recreated the pod again.
- in case the credentials are wrong, `imagePullSecret` needs to be provided. Read secret Management in K8s.
Note: ImagePullBackOff can be divided into two different errors (ImagePull and BackOff). 

## CrashLoopBackOff

