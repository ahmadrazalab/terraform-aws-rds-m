
# AWS RDS Module 🚀

Set up your AWS RDS (Relational Database Service) with ease, including read replicas for improved performance:

- 🗃 **RDS Instances**  
- 🔁 **Read Replicas**  
- 🔒 **Automated Backups**  
- 📊 **Performance Monitoring**  
- 🛠 **Custom Database Configurations**  

## What Does It Do?

This module helps you quickly deploy RDS instances with the option for read replicas:

- **Primary Database**: Create a fully managed RDS instance for your app.  
- **Read Replicas**: Improve read performance by adding one or more read replicas.  
- **Automated Backups**: Keeps your data safe with daily backups.  
- **Monitoring**: Integration with CloudWatch to monitor your RDS instance performance.  

## Getting Started 🚀

### Requirements  
1. **AWS CLI** installed and configured.  
2. **Terraform 1.x+** installed.  
3. **IAM Permissions** for managing RDS instances and snapshots.  

### Example Use

```hcl
module "rds_setup" {
  source          = "./rds-module"
  region          = "us-east-1"
  db_instance_id  = "my-app-db"
  db_instance_type = "db.t3.medium"
  db_engine       = "mysql"
  db_username     = "admin"
  db_password     = "securepassword"
  enable_read_replica = true
}

```

### Outputs  
- ✅ RDS Instance Endpoint  
- ✅ Read Replica Endpoints (if enabled)  
- ✅ DB Instance ID  

## Why Use This Module?

- **Quick Setup**: Deploy an RDS instance with minimal effort.  
- **Scalable**: Add read replicas to distribute read-heavy workloads.  
- **Reliable**: Backups, performance monitoring, and easy scaling make it a solid choice for your database needs.  

---

For more, visit my blog: [docs.ahmadraza.in](https://docs.ahmadraza.in)  
