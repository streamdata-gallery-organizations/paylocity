{
  "info": {
    "name": "Paylocity Get Earning by Earning Code and Start Date",
    "_postman_id": "bb23c09d-f779-4629-aa51-f6332ef46232",
    "description": "Get Earnings returns the single earning with the provided earning code and start date for the selected employee.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V2",
      "item": [
        {
          "id": "9caa3834-3e13-45a2-a32a-9e48568b5548",
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
              "id": "d752bb51-8804-4f77-bc7b-b3db6a0668e4"
            }
          ]
        },
        {
          "id": "6183d720-5b5c-40a6-b3ca-3a3a5497fa52",
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
              "id": "a9695005-8987-440c-877b-d789e891a02c"
            }
          ]
        },
        {
          "id": "281547fd-b1f4-4f1a-a0fd-513742d5565f",
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
              "id": "f05e404a-cc34-4257-8ec5-b09f65e9b51c"
            }
          ]
        }
      ]
    }
  ]
}