# Kontrakty

Plik [contracts.csv](/data/csv/contracts.csv)
zawiera następujące dane:

```csv
Unique Investment Identifier,Business Case ID,Agency Code,Agency Name,Investment Title,Contract ID,Agency Contract ID,Contract Status,Contracting Agency ID,Contract Number (PIID),IDV PIID,IDV Agency ID,Match found in USAspending,Vendor Name (USAspending),Solicitation ID (USAspending),Action Obligation Amount (In $ million) (USAspending),Type of Contract (USAspending),Performance Based Contract (USAspending),Contract Start Date (USAspending),Contract End Date (USAspending),Contract Compete (USAspending),Base Contract ID (USAspending),Identifying Agency ID (USAspending),Transaction Number (USAspending),Timestamp (Contract) Date,Timestamp (Contract) Time,Timestamp (Base Contract) Date,Timestamp (Base Contract) Time
005-000000067,247,5,Department of Agriculture,RMA-02  Corporate Insurance Information Systems (CIIS),22329,,Awarded,4732,GST0011AJ0019,GS00Q09BGD0048,4735,Yes,SCIENCE APPLICATIONS INTERNATIONAL CORPORATION,,29.535882,Cost Plus Award Fee,,01/27/2011,01/30/2016,Y,42210,4732,0,2012-02-29,09:51:39,2012-02-29,09:51:39
005-000001430,248,5,Department of Agriculture,"RMA-04  Infrastructure Modernization, Support and Training (IMST)",22334,,Awarded,4732,GST0011AJ0019,GS00Q09BGD0048,4735,Yes,SCIENCE APPLICATIONS INTERNATIONAL CORPORATION,,29.535882,Cost Plus Award Fee,,01/27/2011,01/30/2016,Y,41352,4732,0,2012-02-28,11:27:33,2012-02-28,11:27:33
...
016-000002145,1054,16,Social Security Administration,Earnings Redesign,19761,,Awarded,2800,SS001060108,,,Yes,LOCKHEED MARTIN CORPORATION,,125.245271,Firm Fixed Price,,09/29/2010,,Y,41774,2800,,2012-02-28,16:26:29,2012-02-28,16:26:29
```

## Źródło danych

http://www.itdashboard.gov/data_feeds (itdashboard.gov/data_feeds)

## Co zostało zrobione?

* Pobranie danych statystycznych (csv)
* Zaimportowanie danych do Google Refine
* Wyczyszczenie danych oraz edycja danych za pomocą Google Refine
* Eksport danych do formatu JSON

## Przykład danych w formacie JSON:
```js
"rows" : [
    {
      "Unique Investment Identifier" : "005-000000067",
      "Business Case ID" : 247,
      "Agency Code" : 5,
      "Agency Name" : "Department of Agriculture",
      "Investment Title" : "RMA-02  Corporate Insurance Information Systems (CIIS)",
      "Contract ID" : 22329,
      "Agency Contract ID" : null,
      "Contract Status" : "Awarded",
      "Contracting Agency ID" : 4732,
      "Contract Number (PIID)" : "GST0011AJ0019",
      "IDV PIID" : "GS00Q09BGD0048",
      "IDV Agency ID" : 4735,
      "Match found in USAspending" : "Yes",
      "Vendor Name (USAspending)" : "SCIENCE APPLICATIONS INTERNATIONAL CORPORATION",
      "Solicitation ID (USAspending)" : null,
      "Action Obligation Amount (In $ million) (USAspending)" : 29.535882,
      "Type of Contract (USAspending)" : "Cost Plus Award Fee",
      "Performance Based Contract (USAspending)" : null,
      "Contract Start Date (USAspending)" : "01/27/2011",
      "Contract End Date (USAspending)" : "01/30/2016",
      "Contract Compete (USAspending)" : "Y",
      "Base Contract ID (USAspending)" : 42210,
      "Identifying Agency ID (USAspending)" : 4732,
      "Transaction Number (USAspending)" : 0,
      "Timestamp (Contract) Date" : "2012-02-29",
      "Timestamp (Contract) Time" : "09:51:39",
      "Timestamp (Base Contract) Date" : "2012-02-29",
      "Timestamp (Base Contract) Time" : "09:51:39"
    },
    {
      "Unique Investment Identifier" : "005-000001430",
      "Business Case ID" : 248,
      "Agency Code" : 5,
      "Agency Name" : "Department of Agriculture",
      "Investment Title" : "RMA-04  Infrastructure Modernization, Support and Training (IMST)",
      "Contract ID" : 22334,
      "Agency Contract ID" : null,
      "Contract Status" : "Awarded",
      "Contracting Agency ID" : 4732,
      "Contract Number (PIID)" : "GST0011AJ0019",
      "IDV PIID" : "GS00Q09BGD0048",
      "IDV Agency ID" : 4735,
      "Match found in USAspending" : "Yes",
      "Vendor Name (USAspending)" : "SCIENCE APPLICATIONS INTERNATIONAL CORPORATION",
      "Solicitation ID (USAspending)" : null,
      "Action Obligation Amount (In $ million) (USAspending)" : 29.535882,
      "Type of Contract (USAspending)" : "Cost Plus Award Fee",
      "Performance Based Contract (USAspending)" : null,
      "Contract Start Date (USAspending)" : "01/27/2011",
      "Contract End Date (USAspending)" : "01/30/2016",
      "Contract Compete (USAspending)" : "Y",
      "Base Contract ID (USAspending)" : 41352,
      "Identifying Agency ID (USAspending)" : 4732,
      "Transaction Number (USAspending)" : 0,
      "Timestamp (Contract) Date" : "2012-02-28",
      "Timestamp (Contract) Time" : "11:27:33",
      "Timestamp (Base Contract) Date" : "2012-02-28",
      "Timestamp (Base Contract) Time" : "11:27:33"
    },
	...
```