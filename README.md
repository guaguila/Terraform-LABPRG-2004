# Terraform configuration for LABPRG-2004

# Introduction

This repository contains the necessary code to configure the gRPC dial-out subscriptions automatically on the spine switch for LABPRG-2004 for CLive 2024.

```markdown
# Terraform Configurations

This repository contains Terraform configurations for setting up telemetry subscriptions on IOS XE devices.

## Files

### cpu.tf
Contains configurations for setting up telemetry subscriptions related to CPU usage metrics.

### header.tf
Defines required providers and authentication details for accessing IOS XE devices.

### terraform.tfvars
Sets variable values used across configurations, including source address, receiver IP, receiver port, and update intervals.

### xpaths.tf
Configures telemetry subscriptions for various device metrics such as environment sensors, interfaces, memory statistics, CDP neighbors, and CPU utilization.

## Variables

- **cpu_periodic**: Short update interval for CPU telemetry.
- **source_address**: Source IP address for telemetry data.
- **receiver_ip**: IP address of the telemetry receiver.
- **receiver_port**: Port to send telemetry data to.
- **example_periodic**: Long update interval for example telemetry subscriptions.
- **subscriptions**: XPath expressions for various telemetry subscriptions.

```
