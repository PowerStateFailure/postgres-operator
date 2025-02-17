---
title: "pgo_scaledown"
---
## pgo scaledown

Scale down a PostgreSQL cluster

### Synopsis

The scale command allows you to scale down a Cluster's replica configuration. For example:

	To list targetable replicas:
	pgo scaledown mycluster --query

	To scale down a specific replica:
	pgo scaledown mycluster --target=mycluster-replica-xxxx

```
pgo scaledown [flags]
```

### Options

```
  -d, --delete-data     Causes the data for the scaled down replica to be removed permanently.
  -h, --help            help for scaledown
      --no-prompt       No command line confirmation.
      --query           Prints the list of targetable replica candidates.
      --target string   The replica to target for scaling down
```

### Options inherited from parent commands

```
      --apiserver-url string     The URL for the PostgreSQL Operator apiserver.
      --debug                    Enable debugging when true.
  -n, --namespace string         The namespace to use for pgo requests.
      --pgo-ca-cert string       The CA Certificate file path for authenticating to the PostgreSQL Operator apiserver.
      --pgo-client-cert string   The Client Certificate file path for authenticating to the PostgreSQL Operator apiserver.
      --pgo-client-key string    The Client Key file path for authenticating to the PostgreSQL Operator apiserver.
```

### SEE ALSO

* [pgo](/operatorcli/cli/pgo/)	 - The pgo command line interface.

###### Auto generated by spf13/cobra on 3-Jun-2019
