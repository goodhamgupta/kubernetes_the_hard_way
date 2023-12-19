# Kubernetes: The Hard Way

Kubernetes implementation based on Kelsey Hightowers [repository](https://github.com/kelseyhightower/kubernetes-the-hard-way). Implemented using AWS instead of GCP.

# Note

Depending on the shell being used, the bash syntax of \${variable\_name} doesn't always work. This caused problems with the CA certificate generation, such as  the following command failing:

```sh
curl --cacert ca.pem https://$\{KUBERNETES_PUBLIC_ADDRESS\}/version
```

One way to avoid this is SSL check is to issue the curl command with `--insecure` or `-k`. However, THIS IS NOT THE RECOMMEND APPROACH.
# Credits

AWS solutions for the repository are available [here](https://github.com/prabhatsharma/kubernetes-the-hard-way-aws).

