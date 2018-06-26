---
name: Paylocity
x-slug: paylocity
description: Paylocity has delivered industry-leading software and unmatched customer
  service since our inception. Our mission of elevating payroll and human resources
  across the backroom and into the boardroom speaks to just that. Today, Paylocity
  continues to develop innovative solutions that simplify the lives of payroll and
  HR professionals across the country. Through powerful analytics, robust reporting,
  intuitive usability, and modern functionality&mdash;our clients increase efficiency
  and manage workforces more effectively.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
x-kinRank: "7"
x-alexaRank: "6810"
tags: Paylocity
created: "2018-06-26"
modified: "2018-06-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/apis.md
specificationVersion: "0.14"
apis:
- name: Paylocity Get All Custom Fields
  x-api-slug: paylocity
  description: Get All Custom Fields for the selected company
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/customfields/{category}
  tags: V2,Companies,CompanyId,Customfields,Category
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidcustomfieldscategory-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidcustomfieldscategory-get-openapi.md
- name: Paylocity Add new employee
  x-api-slug: paylocity
  description: New Employee API sends new employee data directly to Web Pay. Companies
    who use the New Hire Template in Web Pay may require additional fields when hiring
    employees. New Employee API Requests will honor these required fields.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees
  tags: V2,Companies,CompanyId,Employees
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployees-post-openapi.md
- name: Paylocity Get employee
  x-api-slug: paylocity
  description: Get Employee API will return employee data currently available in Web
    Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}
  tags: V2,Companies,CompanyId,Employees,EmployeeId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeid-get-openapi.md
- name: Paylocity Update employee
  x-api-slug: paylocity
  description: Update Employee API will update existing employee data in WebPay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}
  tags: V2,Companies,CompanyId,Employees,EmployeeId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeid-patch-openapi.md
- name: Paylocity Add/update employee's benefit setup
  x-api-slug: paylocity
  description: Sends new or updated employee benefit setup information directly to
    Web Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/benefitSetup
  tags: V2,Companies,CompanyId,Employees,EmployeeId,BenefitSetup
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidbenefitsetup-put-openapi.md
- name: Paylocity Get All Earnings
  x-api-slug: paylocity
  description: Get All Earnings returns all earnings for the selected employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/earnings
  tags: V2,Companies,CompanyId,Employees,EmployeeId,Earnings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearnings-get-openapi.md
- name: Paylocity Add/Update Earning
  x-api-slug: paylocity
  description: Add/Update Earning API sends new or updated employee earnings information
    directly to Web Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/earnings
  tags: V2,Companies,CompanyId,Employees,EmployeeId,Earnings
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearnings-put-openapi.md
- name: Paylocity Get Earnings by Earning Code
  x-api-slug: paylocity
  description: Get Earnings returns all earnings with the provided earning code for
    the selected employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}
  tags: V2,Companies,CompanyId,Employees,EmployeeId,Earnings,EarningCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcode-get-openapi.md
- name: Paylocity Delete Earning by Earning Code and Start Date
  x-api-slug: paylocity
  description: Delete Earning by Earning Code and Start Date
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}
  tags: V2,Companies,CompanyId,Employees,EmployeeId,Earnings,EarningCode,StartDate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-delete-openapi.md
- name: Paylocity Get Earning by Earning Code and Start Date
  x-api-slug: paylocity
  description: Get Earnings returns the single earning with the provided earning code
    and start date for the selected employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/earnings/{earningCode}/{startDate}
  tags: V2,Companies,CompanyId,Employees,EmployeeId,Earnings,EarningCode,StartDate
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidearningsearningcodestartdate-get-openapi.md
- name: Paylocity Get all local taxes
  x-api-slug: paylocity
  description: Returns all local taxes for the selected employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/localTaxes
  tags: V2,Companies,CompanyId,Employees,EmployeeId,LocalTaxes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxes-get-openapi.md
- name: Paylocity Add new local tax
  x-api-slug: paylocity
  description: Sends new employee local tax information directly to Web Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/localTaxes
  tags: V2,Companies,CompanyId,Employees,EmployeeId,LocalTaxes
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxes-post-openapi.md
- name: Paylocity Delete local tax by tax code
  x-api-slug: paylocity
  description: Delete local tax by tax code
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/localTaxes/{taxCode}
  tags: V2,Companies,CompanyId,Employees,EmployeeId,LocalTaxes,TaxCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-delete-openapi.md
- name: Paylocity Get local taxes by tax code
  x-api-slug: paylocity
  description: Returns all local taxes with the provided tax code for the selected
    employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/localTaxes/{taxCode}
  tags: V2,Companies,CompanyId,Employees,EmployeeId,LocalTaxes,TaxCode
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidlocaltaxestaxcode-get-openapi.md
- name: Paylocity Add/update non-primary state tax
  x-api-slug: paylocity
  description: Sends new or updated employee non-primary state tax information directly
    to Web Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/nonprimaryStateTax
  tags: V2,Companies,CompanyId,Employees,EmployeeId,NonprimaryStateTax
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidnonprimarystatetax-put-openapi.md
- name: Paylocity Add/update primary state tax
  x-api-slug: paylocity
  description: Sends new or updated employee primary state tax information directly
    to Web Pay.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/employees/{employeeId}/primaryStateTax
  tags: V2,Companies,CompanyId,Employees,EmployeeId,PrimaryStateTax
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidemployeesemployeeidprimarystatetax-put-openapi.md
- name: Paylocity Get Company-Specific Open API Documentation
  x-api-slug: paylocity
  description: The company-specific Open API endpoint allows the client to GET an
    Open API document for the Paylocity API that is customized with company-specific
    resource schemas. These customized resource schemas define certain properties
    as enumerations of pre-defined values that correspond to the company's setup with
    Web Pay. The customized schemas also indicate which properties are required by
    the company within Web Pay.<br  />To learn more about Open API, click [here](https://www.openapis.org/)
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/companies/{companyId}/openapi
  tags: V2,Companies,CompanyId,Openapi
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2companiescompanyidopenapi-get-openapi.md
- name: Paylocity Obtain new client secret.
  x-api-slug: paylocity
  description: Obtain new client secret for Paylocity-issued client id. See Setup
    section for details.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/credentials/secrets
  tags: V2,Credentials,Secrets
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2credentialssecrets-post-openapi.md
- name: Paylocity Add new employee to Web Link
  x-api-slug: paylocity
  description: Add new employee to Web Link will send partially completed or potentially
    erroneous new hire record to Web Link, where it can be corrected and competed
    by company administrator or authorized Paylocity Service Bureau employee.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api//v2/weblinkstaging/companies/{companyId}/employees/newemployees
  tags: V2,Weblinkstaging,Companies,CompanyId,Employees,Newemployees
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/v2weblinkstagingcompaniescompanyidemployeesnewemployees-post-openapi.md
- name: Paylocity
  x-api-slug: paylocity
  description: Paylocity has delivered industry-leading software and unmatched customer
    service since our inception. Our mission of elevating payroll and human resources
    across the backroom and into the boardroom speaks to just that. Today, Paylocity
    continues to develop innovative solutions that simplify the lives of payroll and
    HR professionals across the country. Through powerful analytics, robust reporting,
    intuitive usability, and modern functionality&mdash;our clients increase efficiency
    and manage workforces more effectively.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28482-paylocity.jpg
  humanURL: http://www.paylocity.com
  baseURL: https://api.paylocity.com//api
  tags: Paylocity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/paylocity/master/_listings/paylocity/openapi.md
x-common:
- type: x-website
  url: http://www.paylocity.com
- type: x-blog
  url: https://www.paylocity.com/resources/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/paylocity
- type: x-github
  url: https://github.com/Paylocity
- type: x-integrations
  url: https://www.paylocity.com/partnerships/integrations/
- type: x-linkedin
  url: https://www.linkedin.com/company/paylocity/
- type: x-twitter
  url: https://twitter.com/Paylocity
- type: x-website
  url: http://paylocity.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---