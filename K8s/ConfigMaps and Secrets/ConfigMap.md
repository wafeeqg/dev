Reference: https://kubernetes.io/docs/concepts/configuration/configmap/

- The ConfigMap is also an API Object in the Kubernetes.
- The ConfigMaps does not provide and secrecy and encryption.
- The purpose of ConfigMap is to store non-confidential configuration data in key-value pairs.
- The Pods can consume ConfigMaps as "Environment Variables", "Command Line Arguments" or "Configuration Files in Volumes".
- The Pods can be parameterised and the ConfigMaps can be fed. This is very helpful as same Image can be run with multiple configurations without making changes in the image file.
- Similar to other objects, the ConfigMap object can also be created from a yaml or json file. But there is one difference that the ConfigMap does not have a `spec` field as other objects like `Pod` or `Deployment`. It has `data`field instead.
- 

