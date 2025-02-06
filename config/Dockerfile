# Use the base image
FROM accelq/accelq-acc-agent:latest
# Set environment variables
ENV agent_name=Cloud_Agent_1 \
    num_concurrent_jobs=1 \
    num_parallel_tc_per_job=3 \
    accelq_server_url=https://saint-gobain.accelq.io/ \
    project_code=FormulaERPMigration \
    tenant_code=saintgobain \
    sharing_type=1 \
    agent_type=Tenant

# Setup environment variables from build arguments
ARG USER_ID
ARG API_KEY

#ENV user_id=$USER_ID \
 #   api_key=$API_KEY
 ENV user_id=${USER_ID}
 ENV api_key=${API_KEY}
    #ddddd
    # Start AccelQ Agent when the container runs
CMD ["sh", "-c", "accelq-agent start"]