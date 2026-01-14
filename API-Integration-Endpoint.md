# API Integration Endpoint

> ℹ️ Last updated: 14 Jan 2026

## Table of Contents
- [About](#about)
- [API Endpoint](#api-endpoint)

---

## About

The API Integration Endpoint provides a comprehensive solution for managing and integrating data 
between SMILE web and mobile applications and other systems, either as a source or destination for 
data exchange, in order to meet the necessary integration requirements. This API supports functions 
such as order integration, post picking order, and manage disposal instruction.

The API Integration functions can only be accessed through a backend-to-backend mechanism. The entire 
integration process takes place entirely on the server side without involving interaction through the 
user interface or frontend. The SMILE system sends and/or receives requests from other systems by 
implementing established authentication and authorization mechanisms. The security mechanisms used may 
include API keys, tokens, signatures, or other mutually agreed-upon security methods. The responses 
received are then processed by the backend client to be stored, analyzed, or forwarded to other systems 
as required for operational needs. This ensures secure data handling, integrated workflows, and 
efficient operational control.

The API Integration Endpoint plays a key role in optimize order management, disposal instruction 
management, improving tracking accuracy, and increasing overall business efficiency. The SMILE system 
have three main integration API such as: SIHA/SITB Integration, WMS Integration, and DIN Integration.

---

## API Endpoint
### SIHA/SITB Integration
| **Type** | **API URL** | **API Name** |
|----------|-------------|--------------|
| POST | /auth/login | Login |
| GET | /v2/order/{key_ssl}/integration | Get Order Integration | 
| GET | /v2/order/{order_id} | Get Order Detail by SMILE Order Id | 
| GET | /v2/orders | Get List Order | 
| GET | /v2/materials | Get Materials | 
| GET | /v2/entities | Get Entities | 
| GET | /v2/manufactures | Get Manufactures | 
| GET | /v2/budget-sources | Get Budget Sources | 
| POST | /v2/order/integration | Create Order Integration | 
| PUT | /v2/order/{key_ssl}/confirm/integration | Confirm Order Integration | 
| PUT | /v2/order/{key_ssl}/cancel/integration | Cancel Order Integration | 

### DIN Integration
| **Type** | **API URL** | **API Name** |
|----------|-------------|--------------|
| POST | /ifp/login | Login |
| POST | /ssl/ifp/picking/order | Post Picking Order | 

### WMS Integration
| **Type** | **API URL** | **API Name** |
|----------|-------------|--------------|
| POST | /auth/login | Login |
| GET | /v2/entities | Get Entities | 
| GET | /v2/provinces | Get Provinces | 
| GET | /v2/regencies | Get Regencies | 
| GET | /v2/materials | Get Materials | 
| GET | /v2/subdistricts | Get Subdistricts | 
| GET | /v2/entity-tags | Get Entity Tags | 
| POST | /wms/disposal/cancellation | Cancel Disposal Instruction |
