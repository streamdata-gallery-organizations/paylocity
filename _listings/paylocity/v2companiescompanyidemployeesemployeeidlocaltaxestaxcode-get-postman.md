{
  "info": {
    "name": "Paylocity Get local taxes by tax code",
    "_postman_id": "bfb66131-5008-4e4b-a1a7-be2e6f254c5a",
    "description": "Returns all local taxes with the provided tax code for the selected employee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V2",
      "item": [
        {
          "id": "6ba3ec73-f190-45af-ab9b-ec01c2354a08",
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
              "id": "9bfd640b-13ea-47cf-8d01-32aef2846035"
            }
          ]
        },
        {
          "id": "52ae8ff7-66f1-42cb-8860-f612dc89aaba",
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
              "id": "588da118-ceec-4c71-931d-fea0612679c6"
            }
          ]
        },
        {
          "id": "769e0724-5f06-45cb-a1e6-492499ff6e93",
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
              "id": "1344d26f-c576-4be3-b0e0-0431bb41a9fe"
            }
          ]
        },
        {
          "id": "c1952418-7c0a-4bce-8c5c-3bdf19087bf6",
          "name": "v2.companies.companyId.employees.employeeId.localTaxes.taxCode.get",
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
            "description": "Returns all local taxes with the provided tax code for the selected employee."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5a69fd48-1454-4324-aa99-ed1268eac49a"
            }
          ]
        },
        {
          "id": "447dec95-f61f-4522-b914-2102ee237711",
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
              "id": "ebdd7eee-97d1-4a2a-a055-89a3b42e2388"
            }
          ]
        }
      ]
    }
  ]
}