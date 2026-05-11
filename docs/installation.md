# Apache APISIX Installation Notes
# Environment
- Linux Server
- Docker-based deployment
- etcd backend
# Basic Steps
- Install Docker
- Deploy etcd
- Configure APISIX
- Start APISIX services
- Verify admin API access
# Verification
curl http://127.0.0.1:9180/apisix/admin/routes
#Notes
- Use separate nodes for production deployments
- Enable monitoring and logging
* Secure admin API endpoints
