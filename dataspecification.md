---
layout: page
title: Specifications
---



  
  <div class="feature">
   
 
  <i class="fa fa-check-square-o" aria-hidden="true"></i>
   Required Fields for clinician demographics:
   <br/>
 <br/>
   
  The following data elements are core data needs and critical requirements for the clinical demographics data proof of concept exercise.  
 
<br/>
 <br/>

 
  </div>



| Line | Required | Column | Description | PI |
|----|---------|--------|----------------------------------------|---------|
| 1 | Required | LastName| MiddleName   |   |
| 2 | Required | FirstName| FirstName   |   |
| 3 | Required | MiddleName| MiddleName |   |
| 4 | Required | Suffix| Suffix         |   |
| 5 | Required | TaxIDindividual | Tax ID number associated with provider (individual practitioner) | Y*         |
| 6 | Required | TaxIDinstitution |Tax ID number associated with provider (institution) For employers, including state and local government agencies and non profit organizations , TIN is the IRS issued employer identification number (EIN). EINS are public information per <a href="https://apps.fcc.gov/coresWeb/html/tin.html">FCC</a> |  |
| 7 | Required | NPI| NPI |    |
| 8 | Required | HCPT Spec Code| Health Care PRovider Taxonomy- Industry standard speciality codes (for complete code list  <a href= "http://www.wpc-edi.com/reference/codelists/healthcare/health-care-provider-taxonomy-code-set/"> see </a> ) |   |
| 9 | Required | isAcceptingPatients| provider is accepting the patients for the payer products: only existing patients, family members of existing patients, new patients, other per Provider/Prayer  |    |
| 10 | Required | PayerNtwkEffDate| Date the provider joined this network. (at the group level for POC purposes) |    |
| 11 | Required | PayerNtwkExpireDate| Date the provider leaved this network. (at the group level for POC purposes) |    |
| 12 | Required | Site/Location EffectiveDate| Provider's start date at this location |    |
| 13 | Required | Site/LocationTerminationDate| Provider's end date at this location  |    |
| 14 | Required | PracticeStreet1 | Provider's place of medical service, practice address street line 1     |    |
| 15 | Required | PracticeStreet2 | Practice address street line 2   |    |
| 16 | Required | PracticeCity| Practice city |    |
| 17 | Required | PracticeState| Practice state |    |
| 18 | Required | PracticeZip| PracticeZip   |    |
| 19 | Required | PracticeTelephone | Practice phone (can he have multiple types by location, ie, appointment, business line )   |    |

<br/>
<br/>
<div class="feature">
           <i class="fa fa-check-square-o" aria-hidden="true"></i>
            Non Critical Data:
              <br/>
              <br/>
        If the data is available, other non-critical data are also requested but not required.  A sampling is listed below
      <br/>
      <br/>
</div>

| Line | Data Needed | Column | Description | PI |
|----|---------|--------|----------------------------------------|---------|
| 20| High | PrimaryContactName| Practice contact name   |   |
| 21| High | PrimaryContactFax  | Fax   |   |
| 22| High | ProviderRetireDate| Date of the provider Retired |   |
| 23| High | ProviderDecreaseDate| Date of the provider decreased         |   |
| 24| High | ProviderProficiencyEnglish| Provider's proficiency in the English language   |   |
| 25| High | ProviderOtherLanguages| Languages spoken by the provider (other than English)   |   |
| 26| High | SiteProficiencyEnglish| Staff proficiency in the English language. |   |


<br/>


