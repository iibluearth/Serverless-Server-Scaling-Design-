# Serverless-Server-Scaling-Design Part 2
<p align="center">
<img src="https://i.imgur.com/Gp1wnwU.png">
</p>

In a serverless architecture, scaling is fully managed by the cloud provider (AWS). AWS Lambda automatically increases or decreases the number of concurrent executions in response to traffic spikes or drops; no manual intervention is required.

Key Benefits:
- Auto-scaling is built-in (no need for Auto Scaling Groups or instance provisioning)
- Infrastructure is abstracted; developers focus on code, not server health

<h2> Traditional vs Serverless</h2> 

Traditional Scaling

- Scaling Method: Manual or Auto Scaling Groups

- Scaling Precision: Instance-level scaling 

- Cost: Pay for uptime (even idle)

- Management Overhead: High - requires patching, monitoring, capacity planning

- Scalability Limits: Limited by instance types and quotas 

Serverless Scaling

- Scaling Method: Automatic, event-driven

- Scaling Precision: Function-level, millisecond-based scaling 

- Cost: Pay per execution (no idle cost)

- Management Overhead: Low - infrastructure is managed by the provider (AWS)

- Scalability Limits: Virtually unlimited (soft concurrency limits can be raised)


