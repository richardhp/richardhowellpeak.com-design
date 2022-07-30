# Design

This repo is to house all the designs

## Infrastructure Overview

This document is to gather my thoughts on how to deploy scalable and secure full-stack web applications using open-source technologies.

## Local Development Environment

IDE plus linting, automation etc.

## Trends

You need processes to learn about and keep up with new developments in technology or tools.

Also beware of using experimental or unstable products that may seem cool and appear to solve lots of problems, only to create more problems due to unstable APIs or pivots in the organisation behind the technology.

## Renting Hardware

The use of terraform for managing actual hard-ware is critical.

Leveraging managed and hosted cloud services instead of self-hosting is also critical.

For test development however, docker-compose run locally would suffice.

## DNS

Managing DNS records, SSL certs etc. etc. is also a requirement.  This should all be automated.

## Automated CI

The CI pipe must be automated, which means services must have an easy and automated way of running tests (including unit tests, api tests, end-to-end tests and load-tests).

This also includes linting and any other code standards.

Then deployments must be automated, which necessitates the use of docker and kubernetes.

## Docker

All services, front and back end, must be dockerised so they can be deployed onto kubernetes.

## Kubernetes

This is a platform that allows for automated deployments.

It can do secret management, autoscaling etc.

## Error Handling

A good strategy for error handling must be designed up-front.

## Logging, metrics and tracing

In order to easily debug services, there must be centralised logging, metrics and tracing.  Metrics are also used to manage auto-scaling.

You also need a simple GUI for managing and searching through logs.

## Kafka

In a lot of cases, communication between services should be done via Kafka.

## Hashicorp Vault

I think the hashicorp vault is useful for lots of situations.

## Storage, Caching and Application Architecture

You then also have to figure out how you are going to store data, in which type of storage (postgres, mongo etc.) and how you are going to manage that within your application.

This all then comes down to the application architecture and the requirements of the project.

## Project Management

Use of Gherkin specs, cards, defect management, ADR, MR etc.

You also need established and enforced software development processes.

## Version control and release notes


## Migrations, roll-outs 

## VPN

Security for development

### The Application

Only once all these pieces of the puzzle are solved, are you ready to start building your application.

Whatever technology you use for this, it makes sense to use the same language for front and back end.  So WASM for any non typescript based projects would seem a good option.

These services must then be dockerised, tested then deployed.

