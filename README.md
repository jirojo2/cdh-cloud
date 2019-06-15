# PoC - CDH on Azure

## 1) Infrastructure with Terraform (on azure)

The ideal state would be to abstract the cloud provider and support also Google Cloud

## 2) Software deployment with Ansible

At this point, the infrastructure should be abstracted.

CDH cannot be fully automated as the cluster has to be configured via GUI on the cloudera manager (to be confirmed), but this step automates most of it.

## 3) Data producer

If we use Kafka as our data bus, this piece would constantly generate data to be consumed by the CDH platform

## 4) Flume consumer

This piece would use Flume to consume the data available on Kafka and make it available on the CDH platform

## 5) Analytics sample

TBD

## Source

https://blog.dbi-services.com/deploy-a-cloudera-cluster-with-terraform-and-ansible-in-azure-part-1/
https://blog.dbi-services.com/deploy-a-cloudera-cluster-with-terraform-and-ansible-in-azure-part-2/
https://blog.dbi-services.com/deploy-a-cloudera-cluster-with-terraform-and-ansible-in-azure-part-3/

https://github.com/cloudera/cloudera-playbook
