_Author_:  <!-- TODO: Add author name --> \
_Created_: <!-- TODO: Add date --> \
_Updated_: <!-- TODO: Add date --> \
_Edition_: Swan Lake

# Sanitation for OpenAPI specification

This document records the sanitation done on top of the official OpenAPI specification from module-ballerinax-tableau. 
The OpenAPI specification is obtained from (TODO: Add source link).
These changes are done in order to improve the overall usability, and as workarounds for some known language limitations.

[//]: # (TODO: Add sanitation details)
1. GET /api/-/pulse/subscriptions/{id}: The parameter id is now marked as required (line 6212).
2. DELETE /api/-/pulse/metrics/{metric_id}: The parameter metric_id is now mandatory (line 5389).
3. GET /api/-/pulse/metrics/{metric_id}: The parameter metric_id is set as required (line 5373).
4. PATCH /api/-/pulse/metrics/{metric_id}: The parameter metric_id has been updated to required (line 5547).
5. DELETE /api/-/pulse/definitions/{definition_id}: The parameter definition_id is now required (line 4491).
6. GET /api/-/pulse/definitions/{definition_id}: The parameter definition_id is now mandatory (line 4518).
7. PATCH /api/-/pulse/definitions/{definition_id}: The parameter definition_id has been marked as required (line 4491).
8. DELETE /api/-/pulse/definitions/{definition_id}/metrics: The parameter definition_id is now required (line 4768).
9. Replace the item type in allowed_granularities array in tableau.metricqueryservice.types.v1.ExtensionOptions which was in a wrong location


## OpenAPI cli command

The following command was used to generate the Ballerina client from the OpenAPI specification. The command should be executed from the repository root directory.

```bash
# TODO: Add OpenAPI CLI command used to generate the client
```
Note: The license year is hardcoded to 2024, change if necessary.