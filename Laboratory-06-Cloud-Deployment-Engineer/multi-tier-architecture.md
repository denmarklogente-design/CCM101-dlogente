# Multi-Tier Architecture

## What is a Two-Tier Architecture?

A Two-Tier Architecture divides an application into two connected parts with different responsibilities. The first part handles the application and user interaction, while the second part manages the data used by the application.

## The Web/Application Tier

The Web/Application Tier is responsible for providing the application interface and responding to requests made by users. It handles HTTP requests and allows users to interact with the system. In this deployment, Nextcloud serves as the Web/Application Tier.

## The Database Tier

The Database Tier is responsible for storing and managing the information needed by the application. It provides persistent storage for application and user data. In this deployment, MariaDB serves as the Database Tier.

## Why Separate Them?

The web server and database are placed in two separate containers because they perform different jobs. Separating them makes the components easier to manage, maintain, and troubleshoot. It also keeps the application and database functions independent from one another.
