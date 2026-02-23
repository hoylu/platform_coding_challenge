# Coding challenge

## Terraform

You are tasked to write terraform code to start multiple docker containers. Two docker containers running a nginx image and three running a plain ubuntu image. The nginx containers should be configured with each a different DNS configuration, a persistent docker volume and access to the internet as well as a private docker network. The ubuntu containers should be configured with a persistent volume, with different sizes, and access to the same private docker network. The ubuntu containers should be kept running. The provided `.tfvars` file can be used as a starting point for this task.

- How would you structure your code to make everything easy to find, extendable and support configuration management?  
- How could you address potential future modifications to the terraform code, like switching the used images or tags, volume sizes or adding additional container instances?  
- What documentation would you create to explain the terraform stack and how it works?
- The guide at this link can be used as a starting point: https://developer.hashicorp.com/terraform/tutorials/docker-get-started/docker-build
