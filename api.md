# BoxFleet hosted control plane (boxfleet.io) C++ API

<!-- omniwrap-api-reference eyJjb250cmFjdF9maW5nZXJwcmludCI6ImUzZmQ0Yzc0NGFlODkzM2MwZTBiZDBjMjFhNjkyODk3Nzk1YTE0NjU3ZTU3N2ZiODIxMDg1MDBkMzlmMmFjOGQiLCJvcGVyYXRpb25fY291bnQiOjU2LCJyZW5kZXJlciI6ImNwcCIsInZlcnNpb24iOiIxLjUuMCJ9 -->

This generated index is tied to Semantic IR `1.14.0` and contract fingerprint `e3fd4c744ae8933c0e0bd0c21a692897795a14657e577fb82108500d39f2ac8d`. Every operation below is rendered from the same semantic contract and artifact-attested public member allocation as the SDK.

SDK maturity: **experimental**  
Artifact evidence: [`omniwrap-artifact.json`](omniwrap-artifact.json) binds this file by SHA-256 and is revalidated by the package gate.

## Shared types

- `HostedPersistentBoxClose`
- `HostedPersistentBoxRead`
- `HostedPersistentUsageMeter`
- `HostedPersistentUsageRead`
- `ObservedBox`

## Resource `accounts`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYWNjb3VudHNfY29uZmlnIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0QWNjb3VudHNDb25maWciLCJwYXRoIjoiL3YxL2FjY291bnRzL2NvbmZpZyIsInJlc291cmNlIjoiYWNjb3VudHMiLCJzZWN0aW9uX3NoYTI1NiI6IjIxZjMxN2M2NTY4MjJhMTU3YzI1ZmEyOTA3YjQ1MTQ0ZDQ0YTJmMDE0MDYyMjEwYTBhYmFkNmEzN2Y3MTg3MDEiLCJzaWduYXR1cmVfc2hhMjU2IjoiMmJjN2MxMTk3N2Q4NWU2NDQ3YjFkNjViMWE2NWVmN2MwNGM2ZmNkNDUxMjdkYjJkN2ExM2MwNDYwMjBmYjM0MSJ9 -->
### `client.get_accounts_config`

Operation ID: `getAccountsConfig`  
Route: `GET` `/v1/accounts/config`  

#### Signature

```cpp
ApiResponse get_accounts_config() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBY2NvdW50c0NvbmZpZyJ9 -->

## Resource `admin`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjb250cm9sX3VzZXIiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY29udHJvbFVzZXIiLCJwYXRoIjoiL3YxL2FkbWluL3VzZXJzIiwicmVzb3VyY2UiOiJhZG1pbiIsInNlY3Rpb25fc2hhMjU2IjoiMGU1M2FiZDgxMjdiYTlmYjIxZTZlYzJjNWVkNWRhYTE3NzM1ZDI1NGI2MTBhYWJmOWJhMmU0NjIxN2M5OWE0OCIsInNpZ25hdHVyZV9zaGEyNTYiOiI1NzdjMTEwZWZkY2QzMmM0NzQ0ODYzZjZhOTcxM2IwNDQ2ODM3Y2JkYTg4ZGZmNzIwYjY0NWUwODUyYWVmZTY0In0 -->
### `client.control_user`

Operation ID: `controlUser`  
Route: `POST` `/v1/admin/users`  

#### Signature

```cpp
ApiResponse control_user(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Applied | none |
| `401` | Admin token required | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjb250cm9sVXNlciJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYWRtaW5fY29uc29sZSIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6ImdldEFkbWluQ29uc29sZSIsInBhdGgiOiIvdjEvYWRtaW4vY29uc29sZSIsInJlc291cmNlIjoiYWRtaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjJjZjk1ZDUwNDQ0NWViOGEzOWI5YmEyOWRmNDg4OTk5OTUxN2RlZTI4MjBkZDY5MTQ5ZmUyZmZmNzM3Mjk4ZWEiLCJzaWduYXR1cmVfc2hhMjU2IjoiNThjZmQxNGE3YjJkMGJiMGNiODYzNDFmYTkzM2M5MjdhMTQ1ZDE1ZDY0MjZiYzc2ZDNiNzg4NWNjYWY3Nzk5NSJ9 -->
### `client.get_admin_console`

Operation ID: `getAdminConsole`  
Route: `GET` `/v1/admin/console`  

#### Signature

```cpp
ApiResponse get_admin_console() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Console | none |
| `401` | Admin token required | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBZG1pbkNvbnNvbGUifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYWRtaW5fcGxhbnMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRBZG1pblBsYW5zIiwicGF0aCI6Ii92MS9hZG1pbi9wbGFucyIsInJlc291cmNlIjoiYWRtaW4iLCJzZWN0aW9uX3NoYTI1NiI6Ijg3Y2NiYmJmNmY2ZjVkNTg4Nzk5MmYwYmYxYjc1ODE1YjYzY2Y5YWQzZWZiNjUyMDM3NmUxYWY5YTcxODNhOWUiLCJzaWduYXR1cmVfc2hhMjU2IjoiOTE0MGZkYjVhMGU0NzFhNzkxNDdiY2NkZTgxYTM2MjBjN2I4YmI3OTJlYjgzMzg2MmM3M2Y0ZDk1MjVhZjEyOSJ9 -->
### `client.get_admin_plans`

Operation ID: `getAdminPlans`  
Route: `GET` `/v1/admin/plans`  

#### Signature

```cpp
ApiResponse get_admin_plans() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Plans | none |
| `401` | Admin token required | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBZG1pblBsYW5zIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X3VzZXJzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdFVzZXJzIiwicGF0aCI6Ii92MS9hZG1pbi91c2VycyIsInJlc291cmNlIjoiYWRtaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjQ4YTA3ZDE1ZjE0YzU4YWFkMjVkZmEwNjllYzIwODZlMjcwYzE2NjQxNDk3YWIxMmFjOTU2ZWYzN2I0M2E0OTMiLCJzaWduYXR1cmVfc2hhMjU2IjoiMWJlMzVmZTgyNDFhNjBhMjcyNDQ0ZmVkM2NmMTIzZWNlYTdjNTM1MzJmZmVjOTFmMThjNWY1ZDUzZGNhMDBjNCJ9 -->
### `client.list_users`

Operation ID: `listUsers`  
Route: `GET` `/v1/admin/users`  

#### Signature

```cpp
ApiResponse list_users() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Users | none |
| `401` | Admin token required | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0VXNlcnMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZWFkX3RlbGVtZXRyeSIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6InJlYWRUZWxlbWV0cnkiLCJwYXRoIjoiL3YxL2FkbWluL3RlbGVtZXRyeSIsInJlc291cmNlIjoiYWRtaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjMwOGVjNTdiZDMwMjg1YjAzYWFkNWIxOGI3M2Y1Zjk1ZDI2YjcwZjJkMmU0NWMwZTMyNWI3MWZlMzUxOTJmZGQiLCJzaWduYXR1cmVfc2hhMjU2IjoiYjgzODc4OTlhMjk4OTRkMmE3ZDA0NzU1ZDYwODZhMWU2NmVkOTk3MTU5MjhkYWZjOGQ3ZjQ4OTQ5ZTFlZDFkZCJ9 -->
### `client.read_telemetry`

Operation ID: `readTelemetry`  
Route: `GET` `/v1/admin/telemetry`  

#### Signature

```cpp
ApiResponse read_telemetry() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Events | none |
| `401` | Admin token required | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWFkVGVsZW1ldHJ5In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJ1cGRhdGVfcGxhbiIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJ1cGRhdGVQbGFuIiwicGF0aCI6Ii92MS9hZG1pbi9wbGFucyIsInJlc291cmNlIjoiYWRtaW4iLCJzZWN0aW9uX3NoYTI1NiI6IjQ0MTZiMWE2M2JmNTU3NTk0MmVkZTQzNGFkYTliYWU0N2U2NTI1MDIyNThmYmNmOGFkZGRkM2U4ZWU2ZTMzY2UiLCJzaWduYXR1cmVfc2hhMjU2IjoiNjkwZGIyNTdiZWU1NzY0NGZhNTQ1ODY1ODdmZWExNTYxZmU2YTc4MjhiYTBiMDhkOTQzZTRkNmZkMjNmZDU4MCJ9 -->
### `client.update_plan`

Operation ID: `updatePlan`  
Route: `POST` `/v1/admin/plans`  

#### Signature

```cpp
ApiResponse update_plan(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Updated | none |
| `401` | Admin token required | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJ1cGRhdGVQbGFuIn0 -->

## Resource `auth`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYXV0aF9nYXRlIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0QXV0aEdhdGUiLCJwYXRoIjoiL3YxL2F1dGgvZ2F0ZSIsInJlc291cmNlIjoiYXV0aCIsInNlY3Rpb25fc2hhMjU2IjoiMDMyNGI5MGJjZTgxYWE5YjA1YzBmZTg3MGM0MGQzNmEwNTI3YWJmZDQ1MDQxZjA5ZjMwNDkwODNiOGZiODI3NyIsInNpZ25hdHVyZV9zaGEyNTYiOiI1ZWUzMTZjMTQ3YWFkMWI5Zjc1NjQwY2I0YWJkZmY4MWEzOTZiNjIyNDk1ZjQ2OTM0YjExYjhjMWIyNTNlOTQyIn0 -->
### `client.get_auth_gate`

Operation ID: `getAuthGate`  
Route: `GET` `/v1/auth/gate`  

#### Signature

```cpp
ApiResponse get_auth_gate() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRBdXRoR2F0ZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZWdpc3RlciIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJyZWdpc3RlciIsInBhdGgiOiIvdjEvYXV0aC9yZWdpc3RlciIsInJlc291cmNlIjoiYXV0aCIsInNlY3Rpb25fc2hhMjU2IjoiNzE0ZjJkZDY1ZmMyMDY0YTE3MTBmODkzN2JhM2EwNjVlOGExYzIyY2MzZWUyZDE3MTZmOTNlYzgyOTgwZWIzMiIsInNpZ25hdHVyZV9zaGEyNTYiOiI2YTIxMDAyNjJkZjk3YzFiM2MxY2U2MDE3ZGE1ZTQxMDQ3NTM4NjY0MDA1Yzc2OGE3ZTkyNTBkMmMzM2FlZjgwIn0 -->
### `client.register`

Operation ID: `register`  
Route: `POST` `/v1/auth/register`  

#### Signature

```cpp
ApiResponse register(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | License issued | none |
| `202` | Verification code sent (or withheld by the resend cooldown) | none |
| `400` | Invalid or expired code | none |
| `403` | Not invited or refused | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |
| `429` | Rate limited | none |
| `503` | Registration not configured | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWdpc3RlciJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJ1cGRhdGVfYXV0aF9nYXRlIiwibWV0aG9kIjoiUFVUIiwib3BlcmF0aW9uX2lkIjoidXBkYXRlQXV0aEdhdGUiLCJwYXRoIjoiL3YxL2F1dGgvZ2F0ZSIsInJlc291cmNlIjoiYXV0aCIsInNlY3Rpb25fc2hhMjU2IjoiNjFmZWRhZjhhNDhhOGEyM2U4NTc4ZWMxMTMxNWI3MmZmMjIzMjAxMDdiMDMzMjM3OTY5MGJmZjIwMzc3ODFlOCIsInNpZ25hdHVyZV9zaGEyNTYiOiI4ODJlYTI5ZDIyMDVjOGU2Nzg3MTg0YTJjMmE0ZGJjZGYxNTJjODliMjU0MjY4ZGJmMjVlMTg4NjE1OTIyZjM3In0 -->
### `client.update_auth_gate`

Operation ID: `updateAuthGate`  
Route: `PUT` `/v1/auth/gate`  

#### Signature

```cpp
ApiResponse update_auth_gate(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Updated | none |
| `401` | Admin token required | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJ1cGRhdGVBdXRoR2F0ZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJ2ZXJpZnlfbGljZW5zZSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJ2ZXJpZnlMaWNlbnNlIiwicGF0aCI6Ii92MS9hdXRoL3ZlcmlmeSIsInJlc291cmNlIjoiYXV0aCIsInNlY3Rpb25fc2hhMjU2IjoiMmUyYWI5NmMxZmVhODVjNmE4MmY0YThmZTdiNzNkYjQzNGU5NWUyY2Q4MzEwNzA4NWVmMWRlMjJiYzdjY2M4YSIsInNpZ25hdHVyZV9zaGEyNTYiOiI1MzI3MTg1ODAwZWQzZmVmMDBmMWM3YjFkZDA5NDE2YzUyYmIwYzE3MWM3MTcyZGI2OGQ1MWQyMTM4NjE0NDFjIn0 -->
### `client.verify_license`

Operation ID: `verifyLicense`  
Route: `POST` `/v1/auth/verify`  

#### Signature

```cpp
ApiResponse verify_license(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Valid | none |
| `401` | Invalid license | none |
| `403` | Refused | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |
| `503` | Verification not configured | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJ2ZXJpZnlMaWNlbnNlIn0 -->

## Resource `billing`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdHJpcGVfd2ViaG9vayIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJzdHJpcGVXZWJob29rIiwicGF0aCI6Ii92MS9iaWxsaW5nL3N0cmlwZS93ZWJob29rIiwicmVzb3VyY2UiOiJiaWxsaW5nIiwic2VjdGlvbl9zaGEyNTYiOiJlZjdlZTg5NTBiOTZiN2NjZjdkNzlmZmFlYzljMTY4NWIxZDkwZDVjZjJkNThjMzA1ODQ1MWExNGNjNzYwMjEyIiwic2lnbmF0dXJlX3NoYTI1NiI6ImZhMTZkMzJiMjg4MzY5YTM2YjFiNTcxMjU0OGEzMjM1N2QxMzE4NzdjZDY3NmUxMmI1YjA2NDRhZjEzNzIyMzUifQ -->
### `client.stripe_webhook`

Operation ID: `stripeWebhook`  
Route: `POST` `/v1/billing/stripe/webhook`  

#### Signature

```cpp
ApiResponse stripe_webhook() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Received | none |
| `400` | Invalid signature or payload | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdHJpcGVXZWJob29rIn0 -->

## Resource `health`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfaGVhbHRoIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0SGVhbHRoIiwicGF0aCI6Ii9oZWFsdGgiLCJyZXNvdXJjZSI6ImhlYWx0aCIsInNlY3Rpb25fc2hhMjU2IjoiNTIzMzBhYjU4MDFmMzM4ZGI5M2U3MTJkNWI4OTg0ZTkxZDNhM2UyODgyNmE5YmY0ZDAyYzBlZjMzYzFkYzM0NiIsInNpZ25hdHVyZV9zaGEyNTYiOiI1ZGY2ODczNTY2ZWUxMTAyMGFiYTJjNWE1NjFlNzUzMTcyY2VlNWQyMWY5MDk2Njc3MDBiODVjMGU2MDkyZjVlIn0 -->
### `client.get_health`

Operation ID: `getHealth`  
Route: `GET` `/health`  

#### Signature

```cpp
ApiResponse get_health() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIZWFsdGgifQ -->

## Resource `jobs`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjYW5jZWxfam9iIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImNhbmNlbEpvYiIsInBhdGgiOiIvdjEvam9icy97am9iSWR9L2NhbmNlbCIsInJlc291cmNlIjoiam9icyIsInNlY3Rpb25fc2hhMjU2IjoiYzcwMDI4YmEwZWFkMWE4ZWU1YjhhMjI1ODQzNmYwZDBlZWVjZmY5ZjliMmVjZmEzMTBlODEwZmQwYzZiZDVhOCIsInNpZ25hdHVyZV9zaGEyNTYiOiI0ZWRlY2E3OTY2MjhhYWQxNDZmYTEwYWJiNjVlYjcxYmJmMTY2MjJmNDliZTQxZmZhMDJkMTk4MDQ4ZGNjN2EzIn0 -->
### `client.cancel_job`

Operation ID: `cancelJob`  
Route: `POST` `/v1/jobs/{jobId}/cancel`  

#### Signature

```cpp
ApiResponse cancel_job(const std::string& arg_0_job_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `jobId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "jobId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjYW5jZWxKb2IifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfam9iIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0Sm9iIiwicGF0aCI6Ii92MS9qb2JzL3tqb2JJZH0iLCJyZXNvdXJjZSI6ImpvYnMiLCJzZWN0aW9uX3NoYTI1NiI6IjhmMmI1ZmExMmM1ODRmMWJkYzg1MzAwMTNjMzAxOGU0YTBjYzJjNWY4YjMxMmI2M2IwZjc4ZDk0ZDVmODIzYjciLCJzaWduYXR1cmVfc2hhMjU2IjoiNjA3ZGNiZjExZWZmZDJiYzQ3MzQ1ZWRiOTNiODdmYzJkYzEwN2VkYTU5ZGI3OGExMTBlNmQ1ZDY5ODlkYmZmMSJ9 -->
### `client.get_job`

Operation ID: `getJob`  
Route: `GET` `/v1/jobs/{jobId}`  

#### Signature

```cpp
ApiResponse get_job(const std::string& arg_0_job_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `jobId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "jobId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRKb2IifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2pvYl9ldmVudHMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJsaXN0Sm9iRXZlbnRzIiwicGF0aCI6Ii92MS9qb2JzL3tqb2JJZH0vZXZlbnRzIiwicmVzb3VyY2UiOiJqb2JzIiwic2VjdGlvbl9zaGEyNTYiOiJiZTNjOGM3OTUwNmEzNDY0OWVmZjdjYTk5NDIwMmMwMTRhMDdhMjg4NjNjOTk3NWVlMjMxY2ZjZDQyYWI3MTZiIiwic2lnbmF0dXJlX3NoYTI1NiI6IjA4MjJmMTg4NmE0NmUzYzU0NGQyM2ZkYTgyMjQ0ZGQ0YzhiOTU1MTJhMzllNzBlOGM3NDZiZjcwMTljMWZhMTAifQ -->
### `client.list_job_events`

Operation ID: `listJobEvents`  
Route: `GET` `/v1/jobs/{jobId}/events`  

#### Signature

```cpp
ApiResponse list_job_events(const std::string& arg_0_job_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `jobId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "jobId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0Sm9iRXZlbnRzIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2pvYnMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJsaXN0Sm9icyIsInBhdGgiOiIvdjEvam9icyIsInJlc291cmNlIjoiam9icyIsInNlY3Rpb25fc2hhMjU2IjoiN2UyYWU4MmNiNzU4NzBjZjFhY2NiNjg2MzkwNmQ3MDVlMDQ4MWU1M2JhZDFlMTgxZmUwY2M3ZDFlZjU1MjczNSIsInNpZ25hdHVyZV9zaGEyNTYiOiIyNDcxODIzYjYyZDU1YTVhNTU3Y2E4YTZlYjYyYTUwOTFiNTU1Njc5ZjExNTc2ZjRmYjVlOWRmNmRkYjhkNDM2In0 -->
### `client.list_jobs`

Operation ID: `listJobs`  
Route: `GET` `/v1/jobs`  

#### Signature

```cpp
ApiResponse list_jobs() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Jobs | none |
| `401` | Session required | none |
| `503` | Storage not configured | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0Sm9icyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdWJtaXRfam9iIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InN1Ym1pdEpvYiIsInBhdGgiOiIvdjEvam9icyIsInJlc291cmNlIjoiam9icyIsInNlY3Rpb25fc2hhMjU2IjoiOGE4ODI2ZGQ2NjAxZDc0MzJkNDg4MzRhNmJlYWU5MTdmYzYzYzViOTlmODIyYTUzMzg3ODY4ZjdlYjIzMjQ4NiIsInNpZ25hdHVyZV9zaGEyNTYiOiJmOGVmYjBjNTM4N2M5MmRjZWJlNDU4NDgzYTg3NTQxNGRhNjgwOTBhYTdkMTcwMzNlOTJjYzU1ZmM2OTg0YjU4In0 -->
### `client.submit_job`

Operation ID: `submitJob`  
Route: `POST` `/v1/jobs`  

#### Signature

```cpp
ApiResponse submit_job(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Replayed | none |
| `201` | Created | none |
| `401` | Session required | none |
| `503` | Storage not configured | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdWJtaXRKb2IifQ -->

## Resource `organizations`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjbG9zZV9wZXJzaXN0ZW50X2JveCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJjbG9zZVBlcnNpc3RlbnRCb3giLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9wZXJzaXN0ZW50LWJveGVzL3tib3hJZH0vY2xvc2UiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjA1NWFlOTY4OWEwMDM3ODY5YzdlMzkyYjcwMTcwYTAwMzkxNThiM2U2YjJmMTU5ZmE5ZDE4YjA2NzYyMzFmMjkiLCJzaWduYXR1cmVfc2hhMjU2IjoiOWM4NGY5NWNhNzM5ZDRkOTJkZTc2YzM4Zjg5MWZlMGNjNjQ3MTRiZTk3Mjg4NGQ5M2VkYWMwOWFmODMzNzU3NCJ9 -->
### `client.close_persistent_box`

Operation ID: `closePersistentBox`  
Route: `POST` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}/close`  

#### Signature

```cpp
ApiResponse close_persistent_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Closure is recorded; repeat requests return the same result without deleting again. | application/json (HostedPersistentBoxClose) |
| `202` | Closure is unconfirmed. Lost, late, negative or mismatched acknowledgements and failed receipt persistence retain reservations. Repeat requests never dispatch another deletion; operator reconciliation is required. | application/json (HostedPersistentBoxClose) |
| `400` | Invalid UUID, body or query parameters. | none |
| `401` | Missing or rejected product session. | none |
| `403` | Current authority denied cleanup or the organization/product/environment differs. | none |
| `404` | No durable box in this exact target scope. | none |
| `409` | Unconfirmed or changed provider allocation requires operator reconciliation. | none |
| `503` | Authority or storage unavailable, or no matching operator provider adapter. Missing configuration refuses before any close intention or deletion. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-c54d-988d0e4e7e77"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjbG9zZVBlcnNpc3RlbnRCb3gifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjcmVhdGVfYmlsbGluZ19wb3J0YWwiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY3JlYXRlQmlsbGluZ1BvcnRhbCIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L2JpbGxpbmcvcG9ydGFsIiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiI0MTFhM2VlMWVhYjY3OTNjNmIwOTQ4OTcxZjRlNDUzMTg1M2RiY2YzZjJkNmE2OTZiY2E4ZjA1ZDRhMTBhMDkzIiwic2lnbmF0dXJlX3NoYTI1NiI6ImE3YjY3MjY0MGJmOGZhMWQ4MDNhZjZjYTg5ODg2NmMxZWQ5YmEzYmI2OTA5MTBmN2U1NDY1NjMxNTk1MzM3NWIifQ -->
### `client.create_billing_portal`

Operation ID: `createBillingPortal`  
Route: `POST` `/v1/organizations/{organizationId}/billing/portal`  

#### Signature

```cpp
ApiResponse create_billing_portal(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | portalUrl | none |
| `404` | No Stripe customer yet | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVCaWxsaW5nUG9ydGFsIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjcmVhdGVfYm94IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImNyZWF0ZUJveCIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L2JveGVzIiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiI0NWMxY2Y0MjRlNWUyNzM1OGZlNDU0MGE0YjBkODI1NDA2NTJmNjY1YjJiYzMyZWFmZDc2MDcwMGIzOWRhYTMwIiwic2lnbmF0dXJlX3NoYTI1NiI6IjE3NDQ2NTBmODVhYjc0N2ZmOWQ4NWI2OGZhMzkzOWYwZWZhOGJiNWMxMTY4MTJkNTM1ODlkMTJhYzA4NWUyMDAifQ -->
### `client.create_box`

Operation ID: `createBox`  
Route: `POST` `/v1/organizations/{organizationId}/boxes`  

#### Signature

```cpp
ApiResponse create_box(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Box running at the provider | none |
| `402` | Concurrent-box limit reached | none |
| `502` | The provider refused; recorded as failed | none |
| `503` | No provider or no storage | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVCb3gifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjcmVhdGVfY2hlY2tvdXQiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoiY3JlYXRlQ2hlY2tvdXQiLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9iaWxsaW5nL2NoZWNrb3V0IiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiIwYzU4Y2ZmNDIyZWU3YmE2OTE0NWEwY2U4ODdhYjFmYjA1MmE2MDlkYjdhMGEyM2NkMjZjMTVlNDkyZDVjOTY3Iiwic2lnbmF0dXJlX3NoYTI1NiI6ImVhYzc0NTEwOGQ4N2IzOWYyYThlNzgxOGUxMTlkZTg0YTkxZmZjNmVkMjMzNTBjMDY3MTZkMzhkNmRiYzZhZDEifQ -->
### `client.create_checkout`

Operation ID: `createCheckout`  
Route: `POST` `/v1/organizations/{organizationId}/billing/checkout`  

#### Signature

```cpp
ApiResponse create_checkout(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | checkoutUrl of the Stripe Checkout Session | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. Autonomous mode: Plan not on sale or subscription exists | none |

#### Canonical required-input example

```json
{
  "body": {
    "planKey": "pro"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjcmVhdGVDaGVja291dCJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYmlsbGluZyIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6ImdldEJpbGxpbmciLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9iaWxsaW5nIiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiJmNmVlZjg3MTFkOWYyZjIyMDExYjAxMTMzZmI1MzYwOTNlYTM1NDljYzE3MDY2ZTMzMzI3YzA3ZmQ5ZGVhMjVmIiwic2lnbmF0dXJlX3NoYTI1NiI6ImUwY2I5NDQ1ZjAwNzU4M2UxOGMxZjYxMjc2MDkzMzJkNGQ2OGI0ZmE0MGY0MjQ1ODQwNGQ3YWQzYzEzM2ZlMWUifQ -->
### `client.get_billing`

Operation ID: `getBilling`  
Route: `GET` `/v1/organizations/{organizationId}/billing`  

#### Signature

```cpp
ApiResponse get_billing(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Billing status | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRCaWxsaW5nIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfYm94IiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0Qm94IiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vYm94ZXMve2JveElkfSIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiZWZmMjk3NTg4YWJjNWNhODhhN2FjOTkzZGI1MmJiZmJhYTU1ZWFlMTViY2E2YjFkY2RhNGVhNzE4NDRiNWM1ZCIsInNpZ25hdHVyZV9zaGEyNTYiOiJmOTNjMWZhMTNkOWI1NjE5NzgwZmZkZmQ4N2RkNWUzMTVjMTE5ZWZhZmM1ZTg0M2FiMjA5ZjZkNTUwMjZiNTZkIn0 -->
### `client.get_box`

Operation ID: `getBox`  
Route: `GET` `/v1/organizations/{organizationId}/boxes/{boxId}`  

#### Signature

```cpp
ApiResponse get_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stored box | none |
| `404` | Unknown box | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-d32a-0e84cb70d88a"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRCb3gifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfZW50aXRsZW1lbnRzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0RW50aXRsZW1lbnRzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vZW50aXRsZW1lbnRzIiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiI5NTNlN2YxYWY3MzQ2ZmExZmU4MTZiZGQ3ZGIzZmNmYzQ4ZGQwZWI1Yzg1YWRkODkxMWZiYTdkMjE1MTRkMDA4Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjYwMWY3MmIzMWJjZmZhZjljYThkMGM2YmZjMGYwZjkyYmFhMDJhOWM1MTI4ODMzN2JlNzAzYzkwZDQ5ZjRjYTgifQ -->
### `client.get_entitlements`

Operation ID: `getEntitlements`  
Route: `GET` `/v1/organizations/{organizationId}/entitlements`  

#### Signature

```cpp
ApiResponse get_entitlements(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Entitlements and usage | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRFbnRpdGxlbWVudHMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfZmxlZXQiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRGbGVldCIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L2ZsZWV0IiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiJjYzIxMWFiOTYzNjk2ZTI0MTY1ZmU1MzAzYWRjZDA0MGVmZDdkYjAxYmUzNzE5YTgxNjcyOWE5YzUzNzM1MGU4Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjI2ZjBiYWYwZjkyZTcxZmYxMDNlMGJhODU3ODEzYzBiYzMyM2ZlMGMxZTExY2YzZGI4YWI4MDQxOWViMzRjODcifQ -->
### `client.get_fleet`

Operation ID: `getFleet`  
Route: `GET` `/v1/organizations/{organizationId}/fleet`  

#### Signature

```cpp
ApiResponse get_fleet(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stored fleet | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRGbGVldCJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfZmxlZXRfcG9saWN5IiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoiZ2V0RmxlZXRQb2xpY3kiLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9mbGVldC9wb2xpY3kiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjRlNTU0Njk5MmQ5ZjAxMTg1ZTQ0YzI4MjEwYWFmZDc0MzNmNmNiNTM5ZmZmODQxZTcxZWI1ZjM4ZjlmY2ViNDciLCJzaWduYXR1cmVfc2hhMjU2IjoiZjFiMWJiODkwZjlhMmEyMDY0YWYwZmQxOTg1YWUyMjU3ZTM1YzQ2YmRkMmMxMGUyNGNjNTk5YjY5MTE0OGYwOSJ9 -->
### `client.get_fleet_policy`

Operation ID: `getFleetPolicy`  
Route: `GET` `/v1/organizations/{organizationId}/fleet/policy`  

#### Signature

```cpp
ApiResponse get_fleet_policy(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Effective policy | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRGbGVldFBvbGljeSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfcGVyc2lzdGVudF9ib3giLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRQZXJzaXN0ZW50Qm94IiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vcGVyc2lzdGVudC1ib3hlcy97Ym94SWR9IiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiJmNThmNzRhZWJkZDAzNThjNjdjMzFmYjBkZGZiM2YxYjU3YzViNWZmYTc4NWIxOGU4MDdhYjBjNzZiNmVkN2JmIiwic2lnbmF0dXJlX3NoYTI1NiI6IjNiYTg5NzQxODgwZmJkMGE0OGJhOTM0MDc0MTQyMTMwOTAyMTg1ZTQxYjQ4YzM3YzU5ODlmMjM1MzY3YzdlMjAifQ -->
### `client.get_persistent_box`

Operation ID: `getPersistentBox`  
Route: `GET` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}`  

#### Signature

```cpp
ApiResponse get_persistent_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Private stored record and reserved budget; runtime status is not-metered. | application/json (object) |
| `400` | Invalid UUID or query parameters. | none |
| `401` | Missing or rejected product session. | none |
| `403` | Current authority denied access or the organization/product/environment differs. | none |
| `404` | No durable box in this exact target scope. | none |
| `503` | Authority or durable record storage unavailable. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-098c-d4f2b24057fb"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRQZXJzaXN0ZW50Qm94In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfcGVyc2lzdGVudF9ib3hfcHJvdmlkZXJfdXNhZ2UiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRQZXJzaXN0ZW50Qm94UHJvdmlkZXJVc2FnZSIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L3BlcnNpc3RlbnQtYm94ZXMve2JveElkfS91c2FnZSIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiYjNhOWExNDZlZTI2MWE2ZjA0ZDJiYThkYjc0OTYyNjVhMmE4MTAwY2JhZTJhYWI0NjY1ZjUyNjZiNWUzNjVkMyIsInNpZ25hdHVyZV9zaGEyNTYiOiI1MjZhYjE1YjcxYjg5ZDE0MzJkMjczZTA0NzkyMjkyNjlkNzExMzUyYjkwYTkzNWRkZjg3ZTc4ZTdhNzVhMTMwIn0 -->
### `client.get_persistent_box_provider_usage`

Operation ID: `getPersistentBoxProviderUsage`  
Route: `GET` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}/usage`  

#### Signature

```cpp
ApiResponse get_persistent_box_provider_usage(const std::string& arg_0_organization_id, const std::string& arg_1_box_id, const QueryItems& query) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `from` | `query` | yes | `string&lt;date-time&gt;` |  |
| `to` | `query` | yes | `string&lt;date-time&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Private provider evidence summary with explicit interval coverage. | application/json (object) |
| `400` | Invalid box ID or bounded UTC window. | none |
| `401` | Missing or rejected product session. | none |
| `403` | Current authority denied access or target scope differs. | none |
| `404` | No durable box in this exact target scope. | none |
| `413` | Stored evidence exceeds the per-read record bound; select a smaller window. | none |
| `503` | Authority or usage storage unavailable. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-0848-7a89fcbe4ab4"
    },
    {
      "in": "query",
      "name": "from",
      "value": "2026-01-01T00:00:00Z"
    },
    {
      "in": "query",
      "name": "to",
      "value": "2026-01-01T00:00:27Z"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRQZXJzaXN0ZW50Qm94UHJvdmlkZXJVc2FnZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2JveGVzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdEJveGVzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vYm94ZXMiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjllYTE2OTc1N2QzMzlkYzJiOTdiOWQ3OTRiYzkyMTVjZGU3NmNkODMwYWFmMjE2NGJmZmU5NzgwMjA3NzBmOGUiLCJzaWduYXR1cmVfc2hhMjU2IjoiZmZjZTUxYmY1Yjg4OGEzYjA4NDkzYmQyODdlNjhlNWY5ZjczMGExNTc5MjhlZTllOTRlMGEyNmJlOGIyOGUxNyJ9 -->
### `client.list_boxes`

Operation ID: `listBoxes`  
Route: `GET` `/v1/organizations/{organizationId}/boxes`  

#### Signature

```cpp
ApiResponse list_boxes(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stored boxes with their provider state | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0Qm94ZXMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2ludm9pY2VzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdEludm9pY2VzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vYmlsbGluZy9pbnZvaWNlcyIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiZTk5MDVhNmZkNTJhMjRkOTk1YmMwN2VhMDYyZWM4ZDRjY2M0MzJkM2MwMjIxMDk3MWVjNjY0ODQ1NWQ5ODc1YiIsInNpZ25hdHVyZV9zaGEyNTYiOiIwZGRhZTM3ODE3OTdmYWEzZmI5MWE0ZjEzNWU0ZDljNDQ4OGE3ZGI3YjRlZmQ1MTk1ZWM5NWE5ZjM4NzA3YjNlIn0 -->
### `client.list_invoices`

Operation ID: `listInvoices`  
Route: `GET` `/v1/organizations/{organizationId}/billing/invoices`  

#### Signature

```cpp
ApiResponse list_invoices(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Invoices | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0SW52b2ljZXMifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X21lbWJlcnMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJsaXN0TWVtYmVycyIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L21lbWJlcnMiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6ImFmNmE2OTA4ODM0NzAyYjA2ODZlYTYwZmE4ZjM1M2U5OGFhY2JiNWNiNTlhMzA5NzA1NjVkYTdiODYzNmNmMjQiLCJzaWduYXR1cmVfc2hhMjU2IjoiZjAxMDI4ODFmMjlmNjZlMWY0ZTFlYjk3YzFhY2RjZjY1YWI0Njg0ODU2NDhkZThhMDljNTBkMTNiMjE3NWUxOCJ9 -->
### `client.list_members`

Operation ID: `listMembers`  
Route: `GET` `/v1/organizations/{organizationId}/members`  

#### Signature

```cpp
ApiResponse list_members(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stored members and the plan seat limit | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0TWVtYmVycyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X29ic2VydmVkX2JveGVzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdE9ic2VydmVkQm94ZXMiLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9vYnNlcnZlZC1ib3hlcyIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiOWJhNTZmNDZhOTkwZDZmOTJlZDBjNWNmM2VjZTI3MDVjZjVhZWYzMzBjNzlkMzhhZGRiYjYzNTJkMjA0NjhjYiIsInNpZ25hdHVyZV9zaGEyNTYiOiJjZDgwYTZiYjkxZTY3ZmMzMjE2NDFhY2I2Y2JkNWM2NzJmNGMxNzUwNTljNzdjZmM1NTg0MWExMzIxZTY3MDViIn0 -->
### `client.list_observed_boxes`

Operation ID: `listObservedBoxes`  
Route: `GET` `/v1/organizations/{organizationId}/observed-boxes`  

#### Signature

```cpp
ApiResponse list_observed_boxes(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Up to 100 non-expired client snapshots, private and not cacheable. | application/json (object) |
| `401` | No valid product session. | none |
| `403` | Organization or scope denied. | none |
| `503` | Inventory storage unavailable. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0T2JzZXJ2ZWRCb3hlcyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X3BlcnNpc3RlbnRfYm94X29mZmVycyIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6Imxpc3RQZXJzaXN0ZW50Qm94T2ZmZXJzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vcGVyc2lzdGVudC1ib3hlcy9vZmZlcnMiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjdlNjYzZWY3OTVhYTYxM2U0ZTgxYTZkYmU3NmE1OGFiMDdjNGI2MjdhZDcxM2EzM2Y1MDNhNTRkNTBkMGY5YmIiLCJzaWduYXR1cmVfc2hhMjU2IjoiMTZlMTFhOGM1OWJmNDU0ZDk4MzBlZjBmNWY1NDFkZmUxM2M0MDA3N2Y5YWM4NjZjZmQ0OWIxZmM3ZWU3YzJjOCJ9 -->
### `client.list_persistent_box_offers`

Operation ID: `listPersistentBoxOffers`  
Route: `GET` `/v1/organizations/{organizationId}/persistent-boxes/offers`  

#### Signature

```cpp
ApiResponse list_persistent_box_offers(const std::string& arg_0_organization_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Private configured offers. | application/json (object) |
| `401` | Product session required. | none |
| `403` | Current read authority denied. | none |
| `503` | Storage or operator offer configuration unavailable. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0UGVyc2lzdGVudEJveE9mZmVycyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X3BlcnNpc3RlbnRfYm94ZXMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJsaXN0UGVyc2lzdGVudEJveGVzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vcGVyc2lzdGVudC1ib3hlcyIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiYTdlNWNjMTI2ZWY4NTI1NWRmZWM3NzM5ZjJjYTkxODJhNzk4Nzg1YTU0ZGQzOGU1YzkxZTVmYWY0ODJiZDNjZiIsInNpZ25hdHVyZV9zaGEyNTYiOiI2ZmJlMjgxZTNiYzAxZDk1MjcwNzczODk2NzM4YzJkYWVlNjVlODcyNTdhNTMzZmJlODY4NzE5YmI3ZDQ3NGI4In0 -->
### `client.list_persistent_boxes`

Operation ID: `listPersistentBoxes`  
Route: `GET` `/v1/organizations/{organizationId}/persistent-boxes`  

#### Signature

```cpp
ApiResponse list_persistent_boxes(const std::string& arg_0_organization_id, const QueryItems& query) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `limit` | `query` | no | `integer` | Maximum recent records; duplicates and other query parameters are rejected. |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Bounded stored records, private and not cacheable. limitReached indicates the requested bound was filled, not an exact total or proof that more records exist. | application/json (object) |
| `400` | Invalid query parameters. | none |
| `401` | Missing or rejected product session. | none |
| `403` | Current authority denied access or the organization/product/environment differs. | none |
| `503` | Authority or durable record storage unavailable. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0UGVyc2lzdGVudEJveGVzIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJwcm92aXNpb25fcGVyc2lzdGVudF9ib3giLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoicHJvdmlzaW9uUGVyc2lzdGVudEJveCIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L3BlcnNpc3RlbnQtYm94ZXMiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjY5MDc2MWUxMWZkMzM2NzI5NGRkOTFmYTk2ZjE4NDllYmJhMTQxODdkNGRiN2U0OTU0ZDg1MjhjNzU1MDlmMGQiLCJzaWduYXR1cmVfc2hhMjU2IjoiMGQ0NWFjZjI0YjU3YmI2ZGZjOTEwNDQ4NDk4NGEwYzNjYjE3NzZlMTFlZThjMmU4ODBhMzlmZjhhMjAyZjAwOCJ9 -->
### `client.provision_persistent_box`

Operation ID: `provisionPersistentBox`  
Route: `POST` `/v1/organizations/{organizationId}/persistent-boxes`  

#### Signature

```cpp
ApiResponse provision_persistent_box(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `Idempotency-Key` | `header` | no | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Previously recorded running or closed allocation; replayed is true. | none |
| `201` | Provider allocation confirmed and recorded as running. Runtime remains reserved, not measured. | application/json (object) |
| `202` | The reservation is held and the allocation remains unconfirmed. Repeated requests never dispatch create again; operator reconciliation is required. | none |
| `400` | Invalid body, unsupported fields, query parameters or idempotency key. | none |
| `401` | Missing or rejected product session. | none |
| `402` | Missing durable entitlement, bounded allowance or available capacity. | none |
| `403` | Current authority denied the operation or target scope. | none |
| `409` | Idempotency conflict, unresolved prior budget or UTC month boundary. | none |
| `413` | Request body exceeds 4 KiB. | none |
| `503` | Authority, storage, operator offer or independent runtime enforcement unavailable. Missing configuration is refused before reservation. | none |

#### Canonical required-input example

```json
{
  "body": {
    "offer": "example",
    "reserveMinutes": 1
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwcm92aXNpb25QZXJzaXN0ZW50Qm94In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJwdXRfZmxlZXRfcG9saWN5IiwibWV0aG9kIjoiUFVUIiwib3BlcmF0aW9uX2lkIjoicHV0RmxlZXRQb2xpY3kiLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9mbGVldC9wb2xpY3kiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjA4NTBiZjBhMjlhY2MwNzQyZmNmOTUyYWZjZDNiYmJmZDU3ZWM1YWI1ZmZmNWU4ODYzYTg3MTc1MDMyMTAzZmUiLCJzaWduYXR1cmVfc2hhMjU2IjoiYjQzY2E2Y2NkNTYyMzg4YjcwYzZjODYxN2MwZjk3NzdmMDFmZjA1ODFhZDUwMDQ0MTNlZTM0ZDQ4MWI5ZWRhYiJ9 -->
### `client.put_fleet_policy`

Operation ID: `putFleetPolicy`  
Route: `PUT` `/v1/organizations/{organizationId}/fleet/policy`  

#### Signature

```cpp
ApiResponse put_fleet_policy(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stored policy | none |
| `400` | Invalid or unenforced field | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJwdXRGbGVldFBvbGljeSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZWNvbmNpbGVfcGVyc2lzdGVudF9ib3giLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoicmVjb25jaWxlUGVyc2lzdGVudEJveCIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L3BlcnNpc3RlbnQtYm94ZXMve2JveElkfS9yZWNvbmNpbGUiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6IjlhZjM3ZTY4OTRmODliZTU3ZjAzMjY3YzY5NjUxMDNhZDEyYTQ4ODczNjhiZGNmMTk3OGRjMTMyNTY2M2M0YmYiLCJzaWduYXR1cmVfc2hhMjU2IjoiMjY5MDI3MjkxNjk2YTU4OWUzZmQyMjY2MzI4ODU4YTVjNDU2ZTRlNTRjMmU4NDY4MDUxZTM1ZjRlY2QzMDgxZSJ9 -->
### `client.reconcile_persistent_box`

Operation ID: `reconcilePersistentBox`  
Route: `POST` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}/reconcile`  

#### Signature

```cpp
ApiResponse reconcile_persistent_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Confirmed operation or replayed receipt. | application/json (object) |
| `202` | Operation remains unconfirmed; reconcile its operation ID without repeating the mutation. | application/json (object) |
| `400` | Invalid bounded lifecycle request. | none |
| `401` | Product session required. | none |
| `402` | Durable feature or quota denied. | none |
| `403` | Fresh operation authority denied. | none |
| `404` | Box or operation missing in the exact organization and deployment. | none |
| `409` | Conflicting operation, unresolved evidence or unavailable runtime budget. | none |
| `503` | Authority, storage or matching operator adapter unavailable. | none |

#### Canonical required-input example

```json
{
  "body": {
    "operationId": "00000000-0000-0000-f735-3d332872b96e"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-a264-3ce9cdfbbeff"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWNvbmNpbGVQZXJzaXN0ZW50Qm94In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZW1vdmVfbWVtYmVyIiwibWV0aG9kIjoiREVMRVRFIiwib3BlcmF0aW9uX2lkIjoicmVtb3ZlTWVtYmVyIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vbWVtYmVycy97dXNlcklkfSIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiYWVhMWQ5ODhhYTUzYmE2YzI2MWI1MTVjMjBjMjYxODlkZGUwMjQ3MDhiNjBlNmZjODA1ODg1ODJlNDRjYzY0YyIsInNpZ25hdHVyZV9zaGEyNTYiOiI2OGI5OTgwNjk3ODJiOWY2NzEwN2ZiNjkwNTkzOTk1MmJkMjRiNmY1NTI0NjBlNjM5ZmZmMWQ5YmJlM2I3Mjc5In0 -->
### `client.remove_member`

Operation ID: `removeMember`  
Route: `DELETE` `/v1/organizations/{organizationId}/members/{userId}`  

#### Signature

```cpp
ApiResponse remove_member(const std::string& arg_0_organization_id, const std::string& arg_1_user_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `userId` | `path` | yes | `string` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Removed | none |
| `404` | Unknown member | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "userId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZW1vdmVNZW1iZXIifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdGFydF9wZXJzaXN0ZW50X2JveCIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJzdGFydFBlcnNpc3RlbnRCb3giLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9wZXJzaXN0ZW50LWJveGVzL3tib3hJZH0vc3RhcnQiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6ImQ3Y2Q0ODdhZTJkYTc2MzdlYjAyZWVlYjRkY2NmZDBiZjY5MDJhNTY0MmNiZDRhODNkNzlkMzMzZjFhYTg3NzQiLCJzaWduYXR1cmVfc2hhMjU2IjoiZmU5YjI0MTU0ZDQ2OWJhYjFkYzYyYzNmMjE0Y2NhODNmNjg0OGMyZWIzZmIyMTJjOWQyMTk1ZDM0NDI1YjE5MiJ9 -->
### `client.start_persistent_box`

Operation ID: `startPersistentBox`  
Route: `POST` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}/start`  

#### Signature

```cpp
ApiResponse start_persistent_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `Idempotency-Key` | `header` | no | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Confirmed operation or replayed receipt. | application/json (object) |
| `202` | Operation remains unconfirmed; reconcile its operation ID without repeating the mutation. | application/json (object) |
| `400` | Invalid bounded lifecycle request. | none |
| `401` | Product session required. | none |
| `402` | Durable feature or quota denied. | none |
| `403` | Fresh operation authority denied. | none |
| `404` | Box or operation missing in the exact organization and deployment. | none |
| `409` | Conflicting operation, unresolved evidence or unavailable runtime budget. | none |
| `503` | Authority, storage or matching operator adapter unavailable. | none |

#### Canonical required-input example

```json
{
  "body": {
    "reserveMinutes": 1
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-d7e8-d81c5e30ed9a"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdGFydFBlcnNpc3RlbnRCb3gifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdG9wX2JveCIsIm1ldGhvZCI6IkRFTEVURSIsIm9wZXJhdGlvbl9pZCI6InN0b3BCb3giLCJwYXRoIjoiL3YxL29yZ2FuaXphdGlvbnMve29yZ2FuaXphdGlvbklkfS9ib3hlcy97Ym94SWR9IiwicmVzb3VyY2UiOiJvcmdhbml6YXRpb25zIiwic2VjdGlvbl9zaGEyNTYiOiI3YzQ0YTM1ZjlkN2JjMzU4YTMyYzNmNjVmMjNkM2MwM2JhNzM2Zjg5MTgzYWU2YjY1Y2M0ZGNlNGVmNGRhOGU4Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjkxYzlhZjJlZjlkNDBmY2E0MWNiNTBhN2I1NzgxODNkZjc3YzgyZWJjOGE3ZGFjYzg5ODA5ZjBiOWZmNzcyMmMifQ -->
### `client.stop_box`

Operation ID: `stopBox`  
Route: `DELETE` `/v1/organizations/{organizationId}/boxes/{boxId}`  

#### Signature

```cpp
ApiResponse stop_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Stopped | none |
| `502` | The provider refused; state unchanged | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-265e-7c895c60153e"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdG9wQm94In0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzdG9wX3BlcnNpc3RlbnRfYm94IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InN0b3BQZXJzaXN0ZW50Qm94IiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vcGVyc2lzdGVudC1ib3hlcy97Ym94SWR9L3N0b3AiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6ImM2NTJlNzhjOGVkYjRkMGUwYTdmODQ4NTJmOTYyZmNkMzY3NzQ5M2RjZGVmYTk4NDMxYjc5OWE4NWRkMGU2Y2YiLCJzaWduYXR1cmVfc2hhMjU2IjoiNGU3ZTUyYzBmYWMwNzg5NmQ5MGMzMTkyMTRmODAwMzdkYzQ3M2UyNGIzMWE0ZDQ0ZDU3Y2FlNDZmOGE1ZmU4OCJ9 -->
### `client.stop_persistent_box`

Operation ID: `stopPersistentBox`  
Route: `POST` `/v1/organizations/{organizationId}/persistent-boxes/{boxId}/stop`  

#### Signature

```cpp
ApiResponse stop_persistent_box(const std::string& arg_0_organization_id, const std::string& arg_1_box_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `boxId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `Idempotency-Key` | `header` | no | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Confirmed operation or replayed receipt. | application/json (object) |
| `202` | Operation remains unconfirmed; reconcile its operation ID without repeating the mutation. | application/json (object) |
| `400` | Invalid bounded lifecycle request. | none |
| `401` | Product session required. | none |
| `402` | Durable feature or quota denied. | none |
| `403` | Fresh operation authority denied. | none |
| `404` | Box or operation missing in the exact organization and deployment. | none |
| `409` | Conflicting operation, unresolved evidence or unavailable runtime budget. | none |
| `503` | Authority, storage or matching operator adapter unavailable. | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    },
    {
      "in": "path",
      "name": "boxId",
      "value": "00000000-0000-0000-978f-a93165cf6579"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzdG9wUGVyc2lzdGVudEJveCJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJzeW5jX29ic2VydmVkX2JveGVzIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InN5bmNPYnNlcnZlZEJveGVzIiwicGF0aCI6Ii92MS9vcmdhbml6YXRpb25zL3tvcmdhbml6YXRpb25JZH0vb2JzZXJ2ZWQtYm94ZXMvc3luYyIsInJlc291cmNlIjoib3JnYW5pemF0aW9ucyIsInNlY3Rpb25fc2hhMjU2IjoiOTJjNjVmOTMyMjk1NTc2NDY1MmI5NjhkNmJiZjkyODA2OWQ3OWZhYTQyNzMxZDYyN2U5ZjM0ZDdmNDBhMDljNiIsInNpZ25hdHVyZV9zaGEyNTYiOiJlODYxNGQyZTE2MzdhZTA5MDEzNGFkOWY0Njk5YTQwMzRlNTY0YzNkM2VjMjMyYjJmYjA4ZmUzYzA3OTVkOTg0In0 -->
### `client.sync_observed_boxes`

Operation ID: `syncObservedBoxes`  
Route: `POST` `/v1/organizations/{organizationId}/observed-boxes/sync`  

#### Signature

```cpp
ApiResponse sync_observed_boxes(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Snapshot accepted; private and not cacheable. | application/json (object) |
| `400` | Invalid observation snapshot. | none |
| `401` | No valid product session. | none |
| `403` | Organization or scope denied. | none |
| `413` | Snapshot exceeds 64 KiB. | none |
| `503` | Inventory storage unavailable. | none |

#### Canonical required-input example

```json
{
  "body": {
    "boxes": [
      {
        "boxId": "example",
        "kind": "provider-list",
        "provider": "example",
        "state": "running"
      }
    ],
    "sourceId": "00000000-0000-0000-ae61-93cfab8e5e4b"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJzeW5jT2JzZXJ2ZWRCb3hlcyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJ1cHNlcnRfbWVtYmVyIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6InVwc2VydE1lbWJlciIsInBhdGgiOiIvdjEvb3JnYW5pemF0aW9ucy97b3JnYW5pemF0aW9uSWR9L21lbWJlcnMiLCJyZXNvdXJjZSI6Im9yZ2FuaXphdGlvbnMiLCJzZWN0aW9uX3NoYTI1NiI6ImE5MjNjYzAwMzgxMDRjNDk3Y2QyOWQ3ZDlkYTk4NTg0MjJkNjk5NDUxYjZmYWZjMWU5ZDY4YmM4OTNhYjY2MTMiLCJzaWduYXR1cmVfc2hhMjU2IjoiNWVhM2UzZTUyZTIxMWEzZDRhYTgzMTQ3YzhkYzQ0NjI2MmQ5MWNmN2JkMmVmZmYxMGQ5M2EwZjExNDU0ZmY2OCJ9 -->
### `client.upsert_member`

Operation ID: `upsertMember`  
Route: `POST` `/v1/organizations/{organizationId}/members`  

#### Signature

```cpp
ApiResponse upsert_member(const std::string& arg_0_organization_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `organizationId` | `path` | yes | `string` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Member updated | none |
| `201` | Member added | none |
| `402` | Seat limit reached or entitlement missing | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "body": {
    "email": "example-f35c@example.test",
    "role": "owner"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "organizationId",
      "value": "example"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJ1cHNlcnRNZW1iZXIifQ -->

## Resource `plans`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfcGxhbnMiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRQbGFucyIsInBhdGgiOiIvdjEvcGxhbnMiLCJyZXNvdXJjZSI6InBsYW5zIiwic2VjdGlvbl9zaGEyNTYiOiI4MzM4NTQ5ZjY3MGZkMGY1NDMzNjMxNjA3M2FhZjEwZjZiZTg5YzMzM2I2NWE1YmQ2YzNiNDM1MGU3ZmNiNmI2Iiwic2lnbmF0dXJlX3NoYTI1NiI6IjFkM2Y1MGUxNDcwMTE0MzE3NDBlMmEzZDUwZjBmOWQ0Y2VkNjg3M2U5ZmFhNGVhY2QxY2I4ZmFmNjMyODc1MTAifQ -->
### `client.get_plans`

Operation ID: `getPlans`  
Route: `GET` `/v1/plans`  

#### Signature

```cpp
ApiResponse get_plans() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | OK | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRQbGFucyJ9 -->

## Resource `telemetry`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJpbmdlc3RfdGVsZW1ldHJ5IiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImluZ2VzdFRlbGVtZXRyeSIsInBhdGgiOiIvdjEvdGVsZW1ldHJ5L2luZ2VzdCIsInJlc291cmNlIjoidGVsZW1ldHJ5Iiwic2VjdGlvbl9zaGEyNTYiOiI4YmYyMjRiNjgxMjI2ZmIyYjk2YWVmMjUzZWM2ZDcwZGZlYWI0YjNkZmEzMDI4MWI5OTVmM2Q0YTdkM2JkZDA0Iiwic2lnbmF0dXJlX3NoYTI1NiI6ImEzN2Q3ZjY4MzMwYjBlNzA5ZTBjMDI0ZDZiYjIzMTE3NGVmYjczNGJiMDIwMjk3MDAzZjc2OGMyZjRhYjg4NDgifQ -->
### `client.ingest_telemetry`

Operation ID: `ingestTelemetry`  
Route: `POST` `/v1/telemetry/ingest`  

#### Signature

```cpp
ApiResponse ingest_telemetry(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `201` | Stored | none |
| `400` | Invalid event | none |
| `401` | License required | none |
| `409` | Managed account authority required; use the returned JackAISaaS accountUrl or portalUrl. | none |
| `413` | Body too large | none |
| `503` | Ingestion not configured | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJpbmdlc3RUZWxlbWV0cnkifQ -->

## Resource `waitlist`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X3dhaXRsaXN0IiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdFdhaXRsaXN0IiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6ImU0NGJmYzQxN2MyZjJjYzM0YTczNTRhNjM4YzBiNzYxN2YyMzk3ZDg4NTcyMWFiNGQ1ZDljYmIyNWUxMGUyMGUiLCJzaWduYXR1cmVfc2hhMjU2IjoiMTRkYjA4ZjYwZWQ1YmQ3ZGIyNGU1YmYwZGM2ZWEyNTg0MDA1YmQ2ZWNkODdlOTE5NGE3N2E2MjQ3NzFlNTA5ZSJ9 -->
### `client.list_waitlist`

Operation ID: `listWaitlist`  
Route: `GET` `/v1/waitlist`  

#### Signature

```cpp
ApiResponse list_waitlist() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Requests | none |
| `401` | Admin token required | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0V2FpdGxpc3QifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZXF1ZXN0X2FjY2VzcyIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJyZXF1ZXN0QWNjZXNzIiwicGF0aCI6Ii92MS93YWl0bGlzdCIsInJlc291cmNlIjoid2FpdGxpc3QiLCJzZWN0aW9uX3NoYTI1NiI6ImVhNjgwZTc2YmFiNGFmZTlhZmI2MzRiNjZmOTUzNjNkNWFkZDlhZWVhZWNkOWE4YTg1YzRhYzkyNjIzMzNlMmUiLCJzaWduYXR1cmVfc2hhMjU2IjoiNzJjZDQyZTQxNjhkNzZkMWQ3NGQ0N2YwZjY5ODViZjMxYWI4YThiYWVjYzY5OTA4MzE5NDQ5ZjA3NjU0NGRmOCJ9 -->
### `client.request_access`

Operation ID: `requestAccess`  
Route: `POST` `/v1/waitlist`  

#### Signature

```cpp
ApiResponse request_access(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `202` | Received | none |
| `400` | Invalid email | none |
| `413` | Body too large | none |
| `429` | Rate limited | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZXF1ZXN0QWNjZXNzIn0 -->

## Resource `workspaces`

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJjbG9zZV9ob3N0ZWRfd29ya3NwYWNlIiwibWV0aG9kIjoiUE9TVCIsIm9wZXJhdGlvbl9pZCI6ImNsb3NlSG9zdGVkV29ya3NwYWNlIiwicGF0aCI6Ii92MS93b3Jrc3BhY2VzL3t3b3Jrc3BhY2VJZH0vY2xvc2UiLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6ImQ1YzNjYzY5NGIxNjc5ZDYyMWUxMDk5MDM0NWI0OGNjNWIzZDRmN2ZiYTExMjVjYTkzNjI1NzE2MDUzMDJmYTAiLCJzaWduYXR1cmVfc2hhMjU2IjoiZWM1MDQ2MmY0Y2E4MGViNDAxNTgxNjQ4YmQ5NTE0YjMwNDFjZTc5YmZhZjdiYjVlNTFkZjViZTMwYjE2YzI2OCJ9 -->
### `client.close_hosted_workspace`

Operation ID: `closeHostedWorkspace`  
Route: `POST` `/v1/workspaces/{workspaceId}/close`  

#### Signature

```cpp
ApiResponse close_hosted_workspace(const std::string& arg_0_workspace_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-6658-e129a559a4dd"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJjbG9zZUhvc3RlZFdvcmtzcGFjZSJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfaG9zdGVkX3dvcmtzcGFjZSIsIm1ldGhvZCI6IkdFVCIsIm9wZXJhdGlvbl9pZCI6ImdldEhvc3RlZFdvcmtzcGFjZSIsInBhdGgiOiIvdjEvd29ya3NwYWNlcy97d29ya3NwYWNlSWR9IiwicmVzb3VyY2UiOiJ3b3Jrc3BhY2VzIiwic2VjdGlvbl9zaGEyNTYiOiJhNTRmZjYzNTkxZDY1OTRlNzk5MTA3MzMzOTBmNjgzNDYyNWQ4OWE3ZTQxZjg3ZmM3MDM5NjQ1NWUyOThkYTU0Iiwic2lnbmF0dXJlX3NoYTI1NiI6ImFiMzYyZTQwMzBiZmY4MjJiYjhkN2FlNTNiYjFjZGNkOTQ4OTdlODNlNmYyZDY2MGViNTk2OGY3MzdmMDcyMzEifQ -->
### `client.get_hosted_workspace`

Operation ID: `getHostedWorkspace`  
Route: `GET` `/v1/workspaces/{workspaceId}`  

#### Signature

```cpp
ApiResponse get_hosted_workspace(const std::string& arg_0_workspace_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-dd2f-cd2edd1eeb24"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIb3N0ZWRXb3Jrc3BhY2UifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfaG9zdGVkX3dvcmtzcGFjZV9vcGVyYXRpb24iLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRIb3N0ZWRXb3Jrc3BhY2VPcGVyYXRpb24iLCJwYXRoIjoiL3YxL3dvcmtzcGFjZXMve3dvcmtzcGFjZUlkfS9vcGVyYXRpb25zL3tvcGVyYXRpb25JZH0iLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6IjI3NDljMWQ2MWMxOGE3MWY0MDJmMThjYjA3ODhhZDRmNzg3ZDczMzNmZjY1MGM2NDAxMjk3ZTk1ZDA4NzI0MDAiLCJzaWduYXR1cmVfc2hhMjU2IjoiYmU2ZDgyMThiNjE5OGZmZmQxZTdhYmUyMmUzMzRjNTI3OWIzN2ZmYWFlZWViZTc3YWNkNzljMGIzZTg4MTU2NCJ9 -->
### `client.get_hosted_workspace_operation`

Operation ID: `getHostedWorkspaceOperation`  
Route: `GET` `/v1/workspaces/{workspaceId}/operations/{operationId}`  

#### Signature

```cpp
ApiResponse get_hosted_workspace_operation(const std::string& arg_0_workspace_id, const std::string& arg_1_operation_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `operationId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-7261-284a8b699ebd"
    },
    {
      "in": "path",
      "name": "operationId",
      "value": "00000000-0000-0000-5ba1-19fa55640b6d"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIb3N0ZWRXb3Jrc3BhY2VPcGVyYXRpb24ifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJnZXRfaG9zdGVkX3dvcmtzcGFjZV9zb3VyY2UiLCJtZXRob2QiOiJHRVQiLCJvcGVyYXRpb25faWQiOiJnZXRIb3N0ZWRXb3Jrc3BhY2VTb3VyY2UiLCJwYXRoIjoiL3YxL3dvcmtzcGFjZXMve3dvcmtzcGFjZUlkfS9zb3VyY2UiLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6Ijc2NWYyNmUwZWQ2MTc1M2U3MjhmYzkwOTcwOGU4MTMyYTgyMTcyNzM3NTkyNjIzMjI5Mjc4M2MyMWZkMGFkZDAiLCJzaWduYXR1cmVfc2hhMjU2IjoiMWI1M2NjMzc4YTdiY2E5ZTM3OTdlMzVjZDFmNzVmMWE1YWJjYzM3NTc0ODMwZTY4MjI0MGY4NzY2YmJjZjZhZSJ9 -->
### `client.get_hosted_workspace_source`

Operation ID: `getHostedWorkspaceSource`  
Route: `GET` `/v1/workspaces/{workspaceId}/source`  

#### Signature

```cpp
ApiResponse get_hosted_workspace_source(const std::string& arg_0_workspace_id) const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-43c8-d895a22336ed"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJnZXRIb3N0ZWRXb3Jrc3BhY2VTb3VyY2UifQ -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJsaXN0X2hvc3RlZF93b3Jrc3BhY2VzIiwibWV0aG9kIjoiR0VUIiwib3BlcmF0aW9uX2lkIjoibGlzdEhvc3RlZFdvcmtzcGFjZXMiLCJwYXRoIjoiL3YxL3dvcmtzcGFjZXMiLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6ImU3M2Q5Y2E1NjM4MWYwYzg5ODNhMmM1YzA1NGU1M2IzYjAyZmZmY2Y5MTFlOTBlMGJiNzhmOWFjNTAzMTUzM2IiLCJzaWduYXR1cmVfc2hhMjU2IjoiOGI1ZDJiZDgyOGU2MzlkZWUwNDBkNjUxZDhhYzZkZmRlMDUyNTk3MmFhMTgyMWJmNDEyNzRjYzJiOGIzOGU4YiJ9 -->
### `client.list_hosted_workspaces`

Operation ID: `listHostedWorkspaces`  
Route: `GET` `/v1/workspaces`  

#### Signature

```cpp
ApiResponse list_hosted_workspaces() const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| _none_ | | | | |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJsaXN0SG9zdGVkV29ya3NwYWNlcyJ9 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJvcGVuX2hvc3RlZF93b3Jrc3BhY2UiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoib3Blbkhvc3RlZFdvcmtzcGFjZSIsInBhdGgiOiIvdjEvd29ya3NwYWNlcyIsInJlc291cmNlIjoid29ya3NwYWNlcyIsInNlY3Rpb25fc2hhMjU2IjoiOWVmMzVkOWUxYWVjN2MwNDBhNWEwNGEyOGEwNjU3ZTY3YzJhN2NmMzBhYzkyMTg3ZmJkOWM0Zjk1NjgzNjFlMyIsInNpZ25hdHVyZV9zaGEyNTYiOiI5OWExNmI1YzRhZDZiZDQxNmQ4NmU0NjQxN2YzOWFkNDc3YWI2NWY3NTMzMjZhM2ZmNjNiMzE0MDE1ZDg1ODhkIn0 -->
### `client.open_hosted_workspace`

Operation ID: `openHostedWorkspace`  
Route: `POST` `/v1/workspaces`  

#### Signature

```cpp
ApiResponse open_hosted_workspace(const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `Idempotency-Key` | `header` | no | `string` | Required here or in the idempotencyKey body field. Replays never allocate or execute again. |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `201` | Prepared workspace; source and provider allocation recorded durably | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "body": {},
  "content_type": "application/json",
  "parameters": []
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJvcGVuSG9zdGVkV29ya3NwYWNlIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJyZWNvdmVyX2hvc3RlZF93b3Jrc3BhY2UiLCJtZXRob2QiOiJQT1NUIiwib3BlcmF0aW9uX2lkIjoicmVjb3Zlckhvc3RlZFdvcmtzcGFjZSIsInBhdGgiOiIvdjEvd29ya3NwYWNlcy97d29ya3NwYWNlSWR9L3JlY292ZXIiLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6IjVmNzE3MDMwY2Q2OGM3OTBkNmQ0ZGRmMTZjM2QyYTM0OTU2M2E0ZmExMmRhNzliNzhiMDljMzk2YjAxY2RkNTEiLCJzaWduYXR1cmVfc2hhMjU2IjoiOWJlN2EyNzBjZTI4N2IyZWZmYTcwZDIzY2Y0MDhhMDAwYjc0OGIyOTkwOWE3OGMzZjI5OGU3NjI1YzY0ZjZhMiJ9 -->
### `client.recover_hosted_workspace`

Operation ID: `recoverHostedWorkspace`  
Route: `POST` `/v1/workspaces/{workspaceId}/recover`  

#### Signature

```cpp
ApiResponse recover_hosted_workspace(const std::string& arg_0_workspace_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `202` | No verified terminal receipt yet; workspace remains unavailable for new commands | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "body": {
    "operationId": "00000000-0000-0000-d4ac-b0b84827b6d9"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-973a-c9ae0260973d"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJyZWNvdmVySG9zdGVkV29ya3NwYWNlIn0 -->

<!-- omniwrap-api-operation eyJleGFtcGxlX3JlYXNvbiI6Imxhbmd1YWdlLWV4YW1wbGUtbm90LWdlbmVyYXRlZCIsImV4YW1wbGVfc3RhdHVzIjoidW5zdXBwb3J0ZWQiLCJtZW1iZXIiOiJydW5faG9zdGVkX3dvcmtzcGFjZSIsIm1ldGhvZCI6IlBPU1QiLCJvcGVyYXRpb25faWQiOiJydW5Ib3N0ZWRXb3Jrc3BhY2UiLCJwYXRoIjoiL3YxL3dvcmtzcGFjZXMve3dvcmtzcGFjZUlkfS9ydW4iLCJyZXNvdXJjZSI6IndvcmtzcGFjZXMiLCJzZWN0aW9uX3NoYTI1NiI6IjE5YTk3ZmUwM2Y0MmQ2NGYwYjA3MzE5YjZiNWRlYjI2NjhmNTZkOGM1OWM1YzI5OGYzNGYwZWI1OTQ2ZmQ0NGMiLCJzaWduYXR1cmVfc2hhMjU2IjoiOWFmOGQ2NGYwYjFkZTE0NWFmMGFkN2Q2ZjhkYzM2ZTcxMGY2ZTU5OTM3MTM4NTA3YWQyOTgyZDAwZTVlNzA5YyJ9 -->
### `client.run_hosted_workspace`

Operation ID: `runHostedWorkspace`  
Route: `POST` `/v1/workspaces/{workspaceId}/run`  

#### Signature

```cpp
ApiResponse run_hosted_workspace(const std::string& arg_0_workspace_id, const std::string& body_json = "") const
```

#### Parameters

| Name | In | Required | Contract type | Description |
| --- | --- | --- | --- | --- |
| `workspaceId` | `path` | yes | `string&lt;uuid&gt;` |  |
| `Idempotency-Key` | `header` | no | `string` | Required here or in the idempotencyKey body field. Replays never allocate or execute again. |
| `body` | body | yes | `object` |  |

#### Responses

| Status | Description | Content |
| --- | --- | --- |
| `200` | Authorized workspace state or result | none |
| `202` | Running or uncertain operation; inspect or explicitly recover, never resend with a new key | none |
| `400` | Invalid bounded request | none |
| `401` | Product session rejected | none |
| `402` | Hub entitlement or atomic quota denied | none |
| `403` | Operation or fleet policy denied | none |
| `404` | Resource not found in the authorized tenant and product environment | none |
| `409` | Idempotency conflict, incompatible state or cleanup unconfirmed | none |
| `503` | Operator provider, template, storage or authority unavailable | none |

#### Canonical required-input example

```json
{
  "body": {
    "command": "example"
  },
  "content_type": "application/json",
  "parameters": [
    {
      "in": "path",
      "name": "workspaceId",
      "value": "00000000-0000-0000-4862-6c003dd1756b"
    }
  ]
}
```

#### SDK call example

Example status: `unsupported`  
Unsupported reason: `language-example-not-generated`

<!-- omniwrap-api-operation-end eyJvcGVyYXRpb25faWQiOiJydW5Ib3N0ZWRXb3Jrc3BhY2UifQ -->

