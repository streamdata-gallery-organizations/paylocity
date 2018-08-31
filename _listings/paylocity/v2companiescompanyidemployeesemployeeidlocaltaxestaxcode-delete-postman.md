{
  "info": {
    "name": "Paylocity Delete local tax by tax code",
    "_postman_id": "d2dc0a71-c49c-47c3-9599-b7b4c4373d73",
    "description": "Delete local tax by tax code",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V2",
      "item": [
        {
          "id": "db4e08bd-7928-4c35-b35a-38115af1cee5",
          "name": "v2.companies.companyId.employees.employeeId.earnings.earningCode.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.paylocity.com",
              "path": [
                "api",
                "v2/companies/:companyId/employees/:employeeId/earnings/:earningCode"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "earningCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "employeeId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer + JWT",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Earnings returns all earnings with the provided earning code for the selected employee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba037b81-d4db-4b1d-944c-7e68c800f8a7"
            }
          ]
        },
        {
          "id": "9b250c89-7779-49c3-b25d-04b0d45fe09e",
          "name": "v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.paylocity.com",
              "path": [
                "api",
                "v2/companies/:companyId/employees/:employeeId/earnings/:earningCode/:startDate"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "earningCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "employeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "startDate",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer + JWT",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get Earnings returns the single earning with the provided earning code and start date for the selected employee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fdd170f9-5121-4355-a883-01e2cf00d56b"
            }
          ]
        },
        {
          "id": "377420a6-1bf5-48dc-84cd-0edee700f928",
          "name": "v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.paylocity.com",
              "path": [
                "api",
                "v2/companies/:companyId/employees/:employeeId/earnings/:earningCode/:startDate"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "earningCode",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "employeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "startDate",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer + JWT",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete Earning by Earning Code and Start Date"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c9cf29a8-e2b1-4085-9274-7ca82e8246bf"
            }
          ]
        },
        {
          "id": "237aba23-eea7-4d60-b12b-9cfc66792956",
          "name": "v2.companies.companyId.employees.employeeId.localTaxes.taxCode.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.paylocity.com",
              "path": [
                "api",
                "v2/companies/:companyId/employees/:employeeId/localTaxes/:taxCode"
              ],
              "variable": [
                {
                  "id": "companyId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "employeeId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "taxCode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer + JWT",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete local tax by tax code"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cdb0e98-0c8a-4cb0-8af8-1715c883e05f"
            }
          ]
        }
      ]
    }
  ]
}