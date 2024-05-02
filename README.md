# Terraform configuration for LABPRG-2004

# Introduction

These files contain the necessary code to configure the gRPC dial-out subscriptions on the LABPRG-2004 for CLive 2024.


```plaintext
## Terraform Configurations

This repository contains Terraform configurations for setting up telemetry subscriptions on IOS XE devices.

### Files

1. **cpu.tf**
   - Configures telemetry subscriptions for CPU data.
   - Subscribes to CPU utilization metrics at different intervals.
   - Utilizes `iosxe_mdt_subscription` resource.
   - Customize update intervals using `cpu_periodic` variable.

2. **header.tf**
   - Defines required providers and credentials.
   - Configures the IOS XE provider with authentication details.
   - Adjust provider version and authentication credentials as needed.

3. **terraform.tfvars**
   - Provides variable values used across configurations.
   - Customize source address, receiver IP, receiver port, and update intervals.

4. **xpaths.tf**
   - Sets up telemetry subscriptions for various device metrics.
   - Subscribes to environment sensors, interfaces, memory statistics, CDP neighbors, and CPU utilization.
   - Adjust subscription XPath expressions and update intervals using variables.

### Variables

- **cpu_periodic**: Short update interval for CPU telemetry.
- **source_address**: Source IP address for telemetry data.
- **receiver_ip**: IP address of the telemetry receiver.
- **receiver_port**: Port to send telemetry data to.
- **example_periodic**: Long update interval for example telemetry subscriptions.
- **subscriptions**: XPath expressions for various telemetry subscriptions.

Ensure to customize variable values and subscription configurations according to your environment requirements.
```
