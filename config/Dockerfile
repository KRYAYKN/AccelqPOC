# Use the base image
FROM accelq/accelq-agent
# Set environment variables
ENV agent_name=SGBCPOCAgent \
    num_concurrent_jobs=1 \
    num_parallel_tc_per_job=3 \
    accelq_server_url=https://poc.accelq.io/ \
    project_code=SaintGobainMSDPOC \
    tenant_code=poc25 \
    sharing_type=1 \
    agent_type=Tenant

# Setup environment variables from build arguments
ARG USER_ID
ARG API_KEY

ENV user_id=$USER_ID \
    api_key=$API_KEY