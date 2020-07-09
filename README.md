# universal-operator
Kubernetes operator to manage any kind of manifest

# Installation
<pre>
$ oc new-project universal-operator
$ oc create -f deploy/crds/saberkan.cloud_universalconfigs_crd.yaml
$ oc create -f deploy/operator.yaml
$ oc create -f deploy/service_account.yaml
$ oc adm policy add-cluster-role-to-user cluster-admin -z universal-operator
</pre>

# Use
<pre>
$ oc create -f deploy/crds/saberkan.cloud_v1alpha1_universalconfig_cr.yaml 
</pre>
