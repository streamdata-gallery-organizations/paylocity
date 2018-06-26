{
  "info": {
    "name": "Paylocity Delete Earning by Earning Code and Start Date",
    "_postman_id": "c6a3bd76-8278-4697-871a-2df96e34ad4b",
    "description": "Delete Earning by Earning Code and Start Date",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "V2",
      "item": [
        {
          "id": "9bf02f04-cb5b-45dd-bde0-1e10b46b4295",
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
              "id": "bb4f811c-5526-43e6-ab18-c2c55890c099"
            }
          ]
        },
        {
          "id": "4858784b-32f0-486b-a3c0-2a49957b8885",
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
              "id": "ecb9e205-d858-4595-a063-86e9de5a1ebf"
            }
          ]
        }
      ]
    }
  ]
}