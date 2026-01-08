# Legacy System Migration to AWS (WordPress on EC2)

## Project Overview
This project demonstrates the migration of a legacy web system to Amazon Web Services (AWS) using a modern cloud-based architecture.  
The goal was to deploy a scalable, secure, and maintainable web application using AWS EC2 and a LAMP stack, with WordPress as the application layer.

Although no real legacy website was provided, this project simulates a real-world migration by building the target environment and documenting the full migration strategy.

---

## Architecture Summary
The system is hosted on a single AWS EC2 instance running Ubuntu Linux.  
The application stack consists of:

- **Apache** – Web server
- **MySQL** – Relational database
- **PHP** – Application runtime
- **WordPress** – Content management system

All components run on the same EC2 instance to reflect a common small-to-medium legacy migration scenario.

An architecture diagram is included in the `/docs` directory.

---

## Technology Stack
- AWS EC2 (Ubuntu)
- Apache 2
- MySQL Server
- PHP
- WordPress
- GitHub (documentation and version control)

---

## Implementation Steps (High Level)

1. Created and configured an AWS EC2 instance
2. Secured access using SSH key pairs
3. Installed and configured the LAMP stack
4. Created and secured a MySQL database
5. Installed and configured WordPress
6. Connected WordPress to the database
7. Verified application availability via public IP
8. Documented migration strategy and architecture

---

## Security Considerations
- SSH access restricted to a single IP
- Database access limited to localhost
- Strong database passwords enforced
- EC2 security groups used as network firewall

---

## Project Outcome
- A fully functional WordPress site running on AWS
- Database successfully connected and tested
- Architecture documented and reproducible
- Migration plan documented for real-world use

---

## Notes
This project focuses on infrastructure setup and migration planning rather than content creation.  
Sample pages may be used to demonstrate functionality, but the emphasis is on backend setup and cloud migration concepts.

---

## Future Improvements
- Use RDS instead of local MySQL
- Add an Application Load Balancer
- Use Terraform for infrastructure provisioning
- Implement CI/CD for automated deployments
