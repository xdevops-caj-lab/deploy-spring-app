[TOC]

# View and working with logs generated by your application


## Logs

OpenShift is constructed in such a way that it expects containers to log all information to STDOUT. In this way, both regular and error information is captured via standardized Docker mechanisms. When exploring the Pod's logs directly, you are essentially going through the Docker daemon to access the container’s logs, through OpenShift’s API.

## View logs on OpenShift web console

Open Pods details page, and check logs.

## View logs via OpenShift CLI

```bash
oc get pods
oc logs -f <pod>
```

Or use [stern](https://github.com/wercker/stern) to view multiple Pods and container logs.
