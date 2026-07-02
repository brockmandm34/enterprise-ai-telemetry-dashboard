# Power BI Data Model Notes

The Power BI dashboard is designed to provide visibility into AI agent operations.

## Suggested Tables

### AgentTelemetry

Main fact table containing one row per AI interaction event.

Example fields:

- timestamp
- agent_name
- session_id
- user_department
- request_type
- latency_ms
- prompt_tokens
- completion_tokens
- estimated_cost_usd
- status
- risk_flag
- feedback_score

### Agent

Dimension table for agent metadata.

Example fields:

- agent_name
- business_owner
- use_case
- risk_tier
- deployment_status

### Department

Dimension table for organizational reporting.

Example fields:

- department_name
- business_unit
- executive_owner

### Date

Standard date table for trend analysis.

## Suggested Dashboard Pages

1. Executive Summary
2. Agent Usage
3. Cost and Token Consumption
4. Performance and Reliability
5. Risk and Safety Events
6. User Feedback

## Example Measures

- Total Requests
- Successful Requests
- Failed Requests
- Failure Rate
- Average Latency
- P95 Latency
- Estimated Cost
- Risk Events
- Average Feedback Score
