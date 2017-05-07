# RS17_project_collection
# collecting  web or desktop applications implemented by Java for RS17 partitioning
# ilustrate each project directories for indexing.

# project name
name=

# index of source code and jar(or bin package for deployment)
src=
bin=

# the directory of source code (exclude test code) for understand parsing;  the directory of original log 
code=
log=

# first stage directory: extract class feature vectors
# source_static:   class_dep.csv from understand parser;  after processing: fv_class_dep.csv and class_dep.rsf 
# source_semantic: fv_class_domain.csv using topic.
# source_dynamic:  method_call.graph; fv_class_commucost.csv with the communication cost as edge weight
# source_trace:    workflow.trace in which, each trace is a complete functionality workflow.
source_static=und.csv,  class.rsf, static_fv.csv
source_semantic=semantic_topic_fv.csv
source_dynamic=dynamic
source_trace=

# second stage directory: partition classes into modules
# partition_static_cluster:  cluster_class_dep_clusternum.csv
# partition_dynamic_cluster: cluster_class_domain_clusternum.csv
# partition_semanti_cluster: cluster_class_commucost_clusternum.csv
partition_static_cluster=
partition_dynamic_cluster=
partition_semanti_cluster=

# third stage directory: identify module service API for servie-service interactions
partition_static_API
partition_dynamic_API
partition_semantic_API

# forth stage directory: identify workflows through services
partition_static_workflow
partition_dynamic_workflow
partition_semantic_workflow
