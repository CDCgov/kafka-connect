Kafka Connect Container for OpenShift 3
=======================================

Version of a popular Kafka Connect Docker image (docker pull spec: confluentinc/cp-kafka-connect)
that will run on OpenShift 3 with the default Security Context Constraint (SCC)
of restricted.

The cp-kafka-connect docker image (at least version 3.3.0) runs fine under the **restricted** SCC already,
so no customization of the image is required at this time.

# Importing Docker image into OpenShift
There is a YAML file in the openshift directory (kafa-connect-imagestream.yml) which will
import the confluentinc/cp-kafka-connect image(s) into the internal registry of an OpenShift
cluster.
