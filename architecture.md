# Architecture Explanation

This deployment uses AWS Fargate as the compute engine for running Docker containers.

The Application Load Balancer distributes incoming HTTP traffic across running tasks.

The ECS Service ensures that one task is always running (replica strategy).

The target group performs health checks to ensure traffic is only sent to healthy containers.

This setup demonstrates a production-style container deployment pattern.
