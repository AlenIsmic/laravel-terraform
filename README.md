── laravel-terraform
  └── terraform                 # our Terraform scripts
    ├── master.tf               # entrypoint for Terraform (TF)
    ├── terraform.tfvars        # TF input variables
    └── modules
      └── vpc                   # VPC configuration
        ├── vpc.tf
        └── outputs.tf
      └── ec2                   # EC2 configuration
        ├── ec2.tf
        └── outputs.tf
      └── aurora                # Aurora configuration
        ├── aurora.tf
        └── outputs.tf
      └── s3                    # S3 configuration
        ├── s3.tf
        └── outputs.tf
  └── cron                      # cron configuration for Docker
    └── artisan-schedule-run
  └── nginx                     # Nginx configuration
    ├── default.conf
    ├── nginx.conf
    └── ssl                     # Nginx SSL certificates
      ├── ssl.cert
      └── ssl.key
  ├── php-fpm                   # PHP-FPM config
  ├── Dockerfile                # Dockerfile for Laravel containers
  ├── Dockerfile-nginx          # Dockerfile for Nginx container
  └── docker-compose.yml        # Docker Compose configuration
