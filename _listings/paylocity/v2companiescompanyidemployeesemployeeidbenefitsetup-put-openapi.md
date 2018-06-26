---
swagger: "2.0"
x-collection-name: Paylocity
x-complete: 0
info:
  title: Paylocity Add/update employee's benefit setup
  description: Sends new or updated employee benefit setup information directly to
    Web Pay.
  termsOfService: WebLink.OpenApiDoc.TermsOfService
  version: "2"
host: api.paylocity.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/companies/{companyId}/customfields/{category}:
    get:
      summary: Get All Custom Fields
      description: Get All Custom Fields for the selected company
      operationId: v2.companies.companyId.customfields.category.get
      x-api-path-slug: v2companiescompanyidcustomfieldscategory-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: category
        description: Custom Fields Category
      - in: path
        name: companyId
        description: Company Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Customfields
      - Category
  /v2/companies/{companyId}/employees:
    post:
      summary: Add new employee
      description: New Employee API sends new employee data directly to Web Pay. Companies
        who use the New Hire Template in Web Pay may require additional fields when
        hiring employees. New Employee API Requests will honor these required fields.
      operationId: v2.companies.companyId.employees.post
      x-api-path-slug: v2companiescompanyidemployees-post
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: body
        name: json
        description: Employee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
  /v2/companies/{companyId}/employees/{employeeId}:
    get:
      summary: Get employee
      description: Get Employee API will return employee data currently available
        in Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeid-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
    patch:
      summary: Update employee
      description: Update Employee API will update existing employee data in WebPay.
      operationId: v2.companies.companyId.employees.employeeId.patch
      x-api-path-slug: v2companiescompanyidemployeesemployeeid-patch
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: Employee Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
  /v2/companies/{companyId}/employees/{employeeId}/benefitSetup:
    put:
      summary: Add/update employee's benefit setup
      description: Sends new or updated employee benefit setup information directly
        to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.benefitSetup.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidbenefitsetup-put
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: employeeId
        description: Employee Id
      - in: body
        name: json
        description: BenefitSetup Model
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - BenefitSetup
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---