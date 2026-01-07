# Architecture Overview

## High-Level Architecture

User requests are sent over the internet to an AWS EC2 instance.
The EC2 instance hosts the entire application stack.

## Components

### EC2 Instance (Ubuntu)
Acts as the main server hosting the application.

### Apache
Handles incoming HTTP requests and serves web pages.

### PHP
Processes application logic required by WordPress.

### MySQL
Stores application data such as posts, users, and settings.

### WordPress
The content management system used by the application.

## Architecture Style
- Single-tier (monolithic)
- All components run on one EC2 instance

## Data Flow
1. User accesses website via browser
2. Request reaches EC2 public IP
3. Apache receives request
4. PHP processes WordPress logic
5. MySQL returns data
6. Response is sent back to user
