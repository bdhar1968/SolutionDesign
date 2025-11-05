
### 1. `LambdaMemory&LoadTest-BDhar.pdf`
A comprehensive technical walkthrough that includes:
- Step-by-step implementation of a serverless pipeline (API Gateway → Lambda → DynamoDB)
- Lambda Power Tuning methodology and memory benchmarking
- Load testing strategy using Postman
- Performance metrics: latency, throughput, and stability
- Key findings and recommendations for cost-efficient scaling

This document serves as both a blueprint and a validation report for optimizing Lambda-based microservices.

### 2. `Postman-Load-test-performance-report1.pdf`  
### 3. `Postman-Load-test-performance-report2.pdf`
These two reports contain raw performance data from Postman load tests run against the optimized Lambda configuration. They include:
- Request/response latency distributions
- Throughput measurements
- Error rates and stability indicators

These files support the findings in the main report and offer transparency into the testing methodology.

## Summary of Findings
This report summarizes key findings from AWS Lambda Power Tuning and Postman load testing of a lambda-over-HTTPS microservice. Performance improved significantly with increased memory, with 512 MB offering the best balance of speed and cost for typical DynamoDB CRUD operations. Load tests revealed stable response times under light concurrency but a 78% error rate under moderate load, pointing to cold starts, throttling, and backend saturation. Recommended optimizations include enabling provisioned concurrency, increasing memory to 512–1024 MB, improving error handling, tuning DynamoDB throughput, and gradually scaling load tests to identify failure thresholds.

---




