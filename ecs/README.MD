Data Source: aws_ecs_cluster
The ECS Cluster data source allows access to details of a specific cluster within an AWS ECS service.

Example Usage
data "aws_ecs_cluster" "ecs-mongo" {
  cluster_name = "ecs-mongo-production"
}


Argument Reference
The following arguments are supported:

cluster_name - (Required) The name of the ECS Cluster
Attributes Reference
In addition to all arguments above, the following attributes are exported:

arn - The ARN of the ECS Cluster
status - The status of the ECS Cluster
pending_tasks_count - The number of pending tasks for the ECS Cluster
running_tasks_count - The number of running tasks for the ECS Cluster
registered_container_instances_count - The number of registered container instances for the ECS Cluster
setting - The settings associated with the ECS Cluster.