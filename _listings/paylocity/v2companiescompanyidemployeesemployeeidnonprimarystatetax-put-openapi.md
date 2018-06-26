---
swagger: "2.0"
x-collection-name: Paylocity
x-complete: 0
info:
  title: Paylocity Add/update non-primary state tax
  description: Sends new or updated employee non-primary state tax information directly
    to Web Pay.
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
  /v2/companies/{companyId}/employees/{employeeId}/earnings:
    get:
      summary: Get All Earnings
      description: Get All Earnings returns all earnings for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearnings-get
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
      - Earnings
    put:
      summary: Add/Update Earning
      description: Add/Update Earning API sends new or updated employee earnings information
        directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.earnings.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearnings-put
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
        description: Earning Model
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
      - Earnings
  /v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}:
    get:
      summary: Get Earnings by Earning Code
      description: Get Earnings returns all earnings with the provided earning code
        for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcode-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
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
      - Earnings
      - EarningCode
  /v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}:
    delete:
      summary: Delete Earning by Earning Code and Start Date
      description: Delete Earning by Earning Code and Start Date
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.delete
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-delete
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: startDate
        description: Start Date
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
      - StartDate
    get:
      summary: Get Earning by Earning Code and Start Date
      description: Get Earnings returns the single earning with the provided earning
        code and start date for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.earnings.earningCode.startDate.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer + JWT
      - in: path
        name: companyId
        description: Company Id
      - in: path
        name: earningCode
        description: Earning Code
      - in: path
        name: employeeId
        description: Employee Id
      - in: path
        name: startDate
        description: Start Date
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - Earnings
      - EarningCode
      - StartDate
  /v2/companies/{companyId}/employees/{employeeId}/localTaxes:
    get:
      summary: Get all local taxes
      description: Returns all local taxes for the selected employee.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxes-get
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
      - LocalTaxes
    post:
      summary: Add new local tax
      description: Sends new employee local tax information directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.post
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxes-post
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
        description: LocalTax Model
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
      - LocalTaxes
  /v2/companies/{companyId}/employees/{employeeId}/localTaxes/{taxCode}:
    delete:
      summary: Delete local tax by tax code
      description: Delete local tax by tax code
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.taxCode.delete
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-delete
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
      - in: path
        name: taxCode
        description: Tax Code
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
      - TaxCode
    get:
      summary: Get local taxes by tax code
      description: Returns all local taxes with the provided tax code for the selected
        employee.
      operationId: v2.companies.companyId.employees.employeeId.localTaxes.taxCode.get
      x-api-path-slug: v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-get
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
      - in: path
        name: taxCode
        description: Tax Code
      responses:
        200:
          description: OK
      tags:
      - V2
      - Companies
      - CompanyId
      - Employees
      - EmployeeId
      - LocalTaxes
      - TaxCode
  /v2/companies/{companyId}/employees/{employeeId}/nonprimaryStateTax:
    put:
      summary: Add/update non-primary state tax
      description: Sends new or updated employee non-primary state tax information
        directly to Web Pay.
      operationId: v2.companies.companyId.employees.employeeId.nonprimaryStateTax.put
      x-api-path-slug: v2companiescompanyidemployeesemployeeidnonprimarystatetax-put
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
        description: Non-Primary State Tax Model
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
      - NonprimaryStateTax
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