---
title: "Data Documentation for k-entry project"
output:
  html_document:
    theme: journal
  pdf_document: default
  word_document: default
---

<script type="text/javascript">
  // When the document is fully rendered...
  $(document).ready(function() {
    // ...select all header elements...
    $('h1, h2, h3, h4, h5').each(function() {
      // ...and add an id to them corresponding to their 'titles'
      $(this).attr('id', $(this).html());
    });
  });
</script>
---

### Quick Links 

<a href="#Variables Used">Go to Variables Used</a><br>
<a href="#Data Source Codes">Go to Data Source Codes</a><br>
<a href="#Level Codes">Go to Level Codes</a>



## Variables Used
|Variable name | Description    | Variable type| Data source |
|:-------------|:---------------|:-------------|:------------|
|GEOID | Census Geography ID | Character | US Census | 
|NAME | Geography name | Character | US Census | 
|county_census | County name from US Census | Character | US Census | 
|  percent_nohighschool_trc | Percentage of census tract residents with no high school diploma | Double | US Census: [Table B06009 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06009) |
|  percent_highschool_trc | Percentage of census tract residents with a high school diploma | Double | US Census: [Table B06009 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06009) |
|  percent_somecollege_trc | Percentage of census tract residents with some college or Associate's degree | Double | US Census: [Table B06009 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06009) |
|  percent_bachelors_trc | Percentage of  census tract residents with a Bachelor’s degree | Double | US Census: [Table B06009 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06009)|
|  percent_gradsch_trc | Percentage of  census tract residentswho have attended graduate school | Double | US Census: [Table B06009 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06009) |
|  percent_mobile14_trc | Percent of  census tract residents who changed geographic location in the past year represented by children age 1 to 4 years old. | Double | US Census: [Table B07001 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B07001) |
|  median_inc_trc | Meadian income of census tract residents in the past 12 months. | Double | US Census: [Table B19326 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&var=B19326001) |
|  percent_healthinsurance_trc | Percent of  census tract residents who have health insurance. | Double | US Census: Table B27003 | https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B27003 |
|  percent_homespre40_trc | Percentage of homes in census tract built before 1940 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes4049_trc | Percentage of homes in census tract built between 1940 - 1949 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes5059_trc | Percentage of homes in census tract built between 1950 - 1959 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes6069_trc | Percentage of homes in census tract built between 1960 - 1969 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes7079_trc | Percentage of homes in census tract geographic area built between 1970 - 1979 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes8089_trc | Percentage of homes in census tract built between 1980 - 1989 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes9099_trc | Percentage of homes in census tract built between 1990 - 1999 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes0009_trc | Percentage of homes in census tract built between 2000 - 2009 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homes1013_trc | Percentage of homes in census tract built between 2010 - 2013 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homespast13_trc | Percentage of homes in census tract built after 2013 | numeric | US Census: [Table B25034 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25034) |
|  percent_homevallt10k_trc | Percentage of homes in census tract valued under $10000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval10to15k_trc | Percentage of homes in census tract valued between $10000 - $15000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval15to20k_trc | Percentage of homes in census tract valued between $15000 - $20000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval20to25k_trc | Percentage of homes in census tract valued between $20000 - 25000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval25to30k_trc | Percentage of homes in census tract valued between $25000 -$30000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval30to35k_trc | Percentage of homes in census tract valued between $30000 - $35000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval35to40k_trc | Percentage of homes in census tract valued between $35000 - $40000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval40to50k_trc | Percentage of homes in census tract valued between $40000 - $50000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval50to60k_trc | Percentage of homes in geographic area valued between $50000 - $60000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval60to70k_trc | Percentage of homes in census tract valued between $60000 - $70000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval70to80k_trc | Percentage of homes in census tract valued between $70000 - $80000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval80to90k_trc | Percentage of homes in census tract valued between $80000 - $90000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval90to100k_trc | Percentage of homes in census tract valued between $90000 - $10000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval100to125k_trc | Percentage of homes in census tract geographic area valued between $100000 - $125000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval125to150k_trc | Percentage of homes in census tract valued between $125000 - $150000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval150to175k_trc | Percentage of homes in census tract valued between $150000 - $175000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval175to200k_trc | Percentage of homes in census tract valued between $175000- $200000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval200to250k_trc | Percentage of homes in census tract valued between $200000 - $250000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval250to300k_trc | Percentage of homes in census tract valued between $250000 - $300000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval300to400k_trc | Percentage of homes in census tract valued between $300000 - $400000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval400to500k_trc | Percentage of homes in census tract valued between $400000 - $500000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval500to750k_trc | Percentage of homes in census tract valued between $500000 - $750000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval750to1000k_trc | Percentage of homes in census tract valued between $750000 - $1000000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval1000to1500k_trc | Percentage of homes in census tract valued between $1000000 - $1500000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homeval1500to2000k_trc | Percentage of homes in census tract valued between $1500000 - $2000000 | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_homevalgt2000k_trc | Percentage of homes in census tract valued over 2 million dollars | numeric | US Census: [Table B25075 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B25075) |
|  percent_englishonly_trc | Percent of  census tract households with English as the only language spoken at home - by ability to speak English for the population 5 years and over | numeric | US Census: [Table B16001 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B16001) |
|  percent_incpovlt1_trc | Percent of  census tract households at or below the national poverty level | numeric | US Census: [Table 05010 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B05010) |
|  percent_incpov12_trc | Percent of  census tract households at 1 to 2 times the national poverty level | numeric | US Census: [Table 05010 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B05010) |
|  percent_incpovgt2_trc | Percent of  census tract households at 2 times the national poverty level | numeric | US Census: [Table 05010 <span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B05010) |
|  year | First year of academic year (e.g., 2015 is from the 2015-16 school year) | Double | kidscount - This is in each linked source of kidscount data. |
|  n_05_children_cou | Number of children in the county between 0-5 years old | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/customreports/5343,5344,5345,5346,5347,5348,5349,5350,5351,5352,5353,5354,5355,5356,5357,5358,5359,5360,5361,5362,5363,5364,5365,5366,5367,5368,5369,5370,5371,5372,5373,5374,5375,5376,5377,5378/any) |
|  n_fostercare_children_cou | Number of children in the county in foster care | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8317-children-in-foster-care?loc=39&loct=5#detailed/5/5343-5378/false/871,870,573,869,36,868,867/any/16894) |
|  n_suppnutrition_children_cou | Child Participants in the Supplemental Nutrition Assistance Program in the county (Number) | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8311-child-participants-in-the-supplemental-nutrition-assistance-program?loc=39&loct=5) |
|  n_tempassist_children_cou | Child Participants in Temporary Assistance for Needy Families in the county (Number) | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8313-child-participants-in-temporary-assistance-for-needy-families?loc=39&loct=5) |
|  n_totaln_children_cou | Total child population in the county | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/102-child-population-by-gender?loc=1&loct=1#detailed/1/any/false/37,871,870,573,869,36,868,867,133,38/14,15,65/421,422) |
|  n_emprelatedaycare_children_cou | Number of children in the county in employment related day care | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8314-child-participants-in-employment-related-day-care#detailed/5/5343-5378/false/37,871,870,573,869,36/any/16891) |
|  per1000_abuseneglect_children_cou | Number of confirmed child victims of abuse or neglect (including Threat of Harm as of 2011) and rate per 1,000 children under age 18 in the county | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2567-abuse-and-neglect-victims?loc=39&loct=5#detailed/5/5343-5378/false/870,573,869,36,868,867,133,38,35,18/any/9861) |
|  per1000_infantmortality_all_cou | Infant mortality in the county (Rate per 1,000) +F51 | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2559-infant-mortality?loc=39&loct=5) |
|  per1000_juvjusref_children_cou | Number of juveniles referred to juvenile courts per 1,000 children ages 0 to 17 in the county | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8340-referrals-to-juvenile-justice?loc=39&loct=5) |
|  per1000_teenpreg1519_all_cou | County rate per 1,000 females ages 15-19 of live births and induced abortions. Oregon teen pregnancy data includes births and induced abortions to teens ages 15-19, 2016. Rate per 1,000 girls ages 15-19. Oregon Health Authority, Health Statistics Unit. “Table 4-3. Pregnancy rates of teens by county of residence, Oregon, 2016.” | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8315-teen-pregnancy-ages-15-to-19?loc=39&loct=5) |
|  percent_adequateprenatcare_all_cou | County percentage of mothers who received prenatal care in the first trimester of their pregnancy | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8888-adequate-prenatal-care?loc=39&loct=5) |
|  percent_ageoutfostercare_children_cou | Children aging out of foster care as a percentage of children exiting foster care in the county | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8320-children-aging-out-of-foster-care?loc=39&loct=5#detailed/5/5343-5378/false/871,870,573,869,36,868,867/any/16897) |
|  percent_amind_all_cou | Percentage of total county population represented by non-Hispanic American Indians or Alaska Natives. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_amind_children_cou | Percentage of county child population represented by non-Hispanic American Indians or Alaska Natives. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_asian_all_cou | Percentage of total county population represented by Asians. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_asian_children_cou | Percentage of county child population represented by Asians. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_black_all_cou | Percentage of total county population represented by Non-hispanic Black people. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_black_children_cou | Percentage of county child population represented by Non-hispanic Black children. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_cohortgrad_children_cou | The percentage of a county's students who receive a regular diploma within four years. Percentage of 2012-13 high school adjusted cohort graduating within four years. Oregon Department of Education, “2015-16 Cohort Graduation Rates.” | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/7185-cohort-graduation-rate?loc=39&loct=5) |
|  n_exitfostercare_children_cou | The number of children who exited foster care in the county | Double | [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8319-children-exiting-foster-care?loc=39&loct=5#detailed/5/5343-5378/false/871,870,573,869,36,868,867/any/16896) |
|  percent_foodinsecure_children_cou | Children under age 18 living in the county in households where in the previous 12 months, there was an uncertainty of having, or an inability to acquire, enough food for all household members because of insufficient money or other resources. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8332-children-in-food-insecure-households?loc=39&loct=5) |
|  percent_fostercare_children_cou | Children spending at least one day in foster care as a percentage of the county's child population (ages 0 to 17) | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8318-percentage-of-children-in-foster-care?loc=39&loct=5#detailed/5/5343-5378/false/871,870,573,869,36,868,867/any/16895) |
|  percent_frl_children_cou | Percent of the county's public school students eligible for free or reduced price lunches. Eligibility criteria is family income less than 185% of the federal poverty level. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8338-students-eligible-for-free-or-reduced-lunch?loc=39&loct=5#detailed/5/5343-5378/false/1740,1639,1600,1536,1460,1249,1120,1024/any/16922) |
|  percent_g3mathprof_children_cou | Percentage of 3rd grade students in the county who met or exceeded state standards in math | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2552-3rd-grade-math-proficiency?loc=39&loct=5) |
|  percent_g3readprof_children_cou | Percentage of 3rd grade students in the county who met or exceeded state standards in reading | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2551-3rd-grade-reading-proficiency?loc=39&loct=5) |
|  percent_g8mathprof_children_cou | Percentage of 8th grade students in the county who met or exceeded state standards in math | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2554-8th-grade-math-proficiency?loc=39&loct=5) |
|  percent_g8readprof_children_cou | Percentage of 8th grade in the county students who met or exceeded state standards in reading | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2553-8th-grade-reading-proficiency?loc=39&loct=5) |
|  percent_hispanic_all_cou | Percentage of total population in the county represented by Hispanics. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_hispanic_children_cou | Percentage of county child population represented by Hispanics. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_homeless_children_cou | The percentage of students in the county who lack a fixed, regular, and adequate nighttime residence during the academic year. A student is identified as homeless when they live in emergency shelter or share housing with others due to loss of housing or economic hardship and/or stay at motels or live in cars, parks, public places, tents, trailers, or other similar settings. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/7186-homeless-students?loc=39&loct=5) |
|  percent_immuniz4313_childre_coun | Percentage of two-year-olds in the county being up to date for their 4:3:1:3 immunization series | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2561-immunizations-4313-series?loc=39&loct=5) |
|  percent_immuniz4313314_children_cou | Percentage of two-year-olds in the county being up to date for their 4:3:1:3:3:1:4 immunization series. note: Gilliam, Sherman, and Wasco counties report as one region | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8889-immunizations-4313314-series?loc=39&loct=5) |
|  percent_multi_all_cou | Percentage of total county population represented by non-Hispanic bi-racial and multi-racial people. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_multi_children_cou | Percentage of county child population represented by non-Hispanic bi-racial and multi-racial children. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_nohealthinsur_children_cou | Percentage of children ages 0-17 in the county estimated to be without health insurance. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2560-children-without-health-insurance?loc=39&loct=5) |
|  percent_noschoolage34_children_cou | Percentage of children ages 3 to 4 in the county not enrolled in school. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8339-children-ages-3-to-4-not-enrolled-in-school?loc=39&loct=5) |
|  percent_pacisl_all_cou | Percentage of total county population represented by non-Hispanic Native Hawaiians/Pacific Islanders. | Double | BRT [kidscount <span style="color:black"> </span>](| https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_pacisl_children_cou | Percentage of county child population represented by non-Hispanic Native Hawaiian/Pacific Islander children. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  percent_poverty_children_cou | Percentage of children in the county estimated to live in families with incomes at or below 100% of the Federal Poverty Level | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2564-childhood-poverty?loc=39&loct=5) |
|  percent_stablefostercare_children_cou | Percentage of children in foster care in the county with two or fewer placement settings. NOTE: County stability rates were calculated only for youth on the last day of the fiscal year, whereas the state rate was calculated for youth spending at least one day in care at any point during the year. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/2570-foster-care-placement-stability?loc=39&loct=5) |
|  percent_unemployed_all_cou | Percent of county population unemployed | Double | BRT kidscount |  |
|  percent_white_all_cou | Percentage of total county population represented by non-Hispanic white people. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8308-total-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16886) |
|  percent_white_children_cou | Percentage of county child population represented by non-Hispanic white children. | Double | BRT [kidscount <span style="color:black"> </span>](https://datacenter.kidscount.org/data/tables/8307-child-population-by-race?loc=39&loct=5#detailed/5/5343-5378/false/37,871,870,573,869,36,868,867,133/1,2,1310,142,4370,4371,3/16885) |
|  county | County | Character | kidscount | This is in each linked source of kidscount data |
|  ncessch | School identification number | Double | NCES; BRT nces-dataprep.R |
|  state | Reported location state, abbreviation | Character | NCES; BRT nces-dataprep.R |
|  cbsa | Core Based Statistical Area | Character | NCES; BRT nces-dataprep.R |
|  cbsatype | Metropolitan or Micropolitan Statistical Area Indicator | Character | NCES; BRT nces-dataprep.R |
|  cnty | FIPS county code | Double | NCES | BRT nces-dataprep.R |
|  fipst | FIPS state code | Double | NCES | BRT nces-dataprep.R |
|  statename | Reported location state, full name | Character | NCES; BRT nces-dataprep.R |
|  sch_name | School name | Character | NCES | BRT nces-dataprep.R |
|  lea_name | local education agency (school dstrict) name | Character | NCES; BRT nces-dataprep.R |
|  st_leaid | State assigned local education agency (school dstrict) ID | Character | NCES; BRT nces-dataprep.R |
|  leaid | NCES assigned local education agency (school dstrict) ID | Double | NCES; BRT nces-dataprep.R |
|  st_schid | State assigned school ID | Character | NCES; BRT nces-dataprep.R |
|  sy_status_text | School Status. 8 levels: "Open" , New", "Closed", "Reopened", "Future", "Changed Boundary", "Added", "Changed Agency" | Character | NCES | BRT nces-dataprep.R |
|  sch_type_text | Type of school. 4 levels: "Regular School", "Special Education School", "Alternative School", "Alternative Education School" | Character | NCES; BRT nces-dataprep.R |
|  recon_status | Whether school is on reconstruction status | Character | NCES; BRT nces-dataprep.R |
|  charter_text | Whether school is a charter school | Character | NCES; BRT nces-dataprep.R |
|  g_pk_offered | Whether school offers pre-K | Character | NCES; BRT nces-dataprep.R |
|  tot_enrollment_sch | Total school enrollment | Double | NCES; BRT nces-dataprep.R |
|  teacher_fte | The full time equivalency of the teachers at the school. | Double | NCES; BRT nces-dataprep.R |
|  prop_frl_sch | Proportion of school's student population receiving free or reduced price lunch. | Double | NCES; BRT nces-dataprep.R |
|  re_amind_sch | Percentage of school's student population represented by American Indian children | Double | NCES; BRT nces-dataprep.R |
|  re_asian_sch | Percentage of school's student population represented by Asian-American children | Double | NCES; BRT nces-dataprep.R |
|  re_black_sch | Percentage of school's student population represented by non-Hispanic Black children | Double | NCES; BRT nces-dataprep.R |
|  re_hisp_sch | Percentage of school's student population represented by Hispanic children | Double | NCES; BRT nces-dataprep.R |
|  re_missing_sch | Percentage of school's student population with race/ethnicity info missing. | Double | NCES; BRT nces-dataprep.R |
|  re_multi_sch | Percentage of school's student population represented by non-Hispanic bi-racial and multi-racial children | Double | NCES; BRT nces-dataprep.R |
|  re_nathi_sch | Percentage of school's student population represented by Native Hawaiian or Other Pacific Islander children | Double | NCES; BRT nces-dataprep.R |
|  re_white_sch | Percentage of school's student population represented by non-Hispanic white children | Double | NCES; BRT nces-dataprep.R |
|  prop_gen_female_sch | Proportion of school's student population identified as female | Double | NCES; BRT nces-dataprep.R |
|  prop_gen_miss_sch | Proportion of school's student population with gender info missing | Double | NCES; BRT nces-dataprep.R |
|  self_reg_av_ind | Individual Student's average rating on CBRS self-regulation items | Double | OKA; al_s_ravg |
|  interpersonal_ind | Individual Student's average rating on CBRS interpersonal skills items | Double | OKA; al_i_savg |
|  gender_ind | gender | Character | OKA |
|  ethnic_cd_ind	| Code representing the student's racial/ethnic reporting subgroup category. A = Asian race, non-Hispanic; B = Black/African American race, non-Hispanic; H = Hispanic ethnicity; I = American Indian/Alaskan Native race, non-Hispanic; M = Multi-racial, non-Hispanic; P = Pacific Islander race, non-Hispanic; W = White race, non-Hispanic	| Character |	OKA |
|  a_schl_id | ODE assigned Institution Identifier for the Attending School. The School where the student is receiving instruction and where state assessments are administered. | Double | OKA; aDistID |
|  a_dist_id | ODE assigned Institution Identifier for the Attending District. The District where the student is receiving instruction and where state assessments are administered. | Double | OKA; aSchlID |
|  math_score_ind | Individual Student's Early Math Score | Double | OKA | EMa_TOTscore |
|  ln_uppercase_score_ind | Individual Student's English uppercase letter names score | Double | BRT OKA; OKA section of data-combine.R |
|  ln_lowercase_score_ind | Individual Student's English lowercase letter names score | Double | BRT OKA; OKA section of data-combine.R |
|  ls_ind | Individual Student's English letter sounds score | Double | BRT OKA; OKA section of data-combine.R |
|  ln_ind | Individual Student's English letter names score | Double | BRT OKA; OKA section of data-combine.R |
|  ssid_ind | Individual Student's Current Secure Student Identifier (SSID). | Double | OKA; RptChkDigitStdntID |
|  lat | Latitiude of school location | Double | [NCES <span style="color:black"> </span>](https://nces.ed.gov/programs/edge/Geographic/SchoolLocations) |
|  lon | Longitude of school location | Double | [NCES <span style="color:black"> </span>](https://nces.ed.gov/programs/edge/Geographic/SchoolLocations) |
|  geometry |  | List | US Census |
| pop_est_trc	 | Estimated total population	| Double | US Census: [Table B01003 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B01003)
| gini_est_trc | Estimated gini coefficient | Double | US Census: [Table B19083 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19083)
| pop_15up_trc |	Estimated total population age 15 and older | Double | US Census: [Table B06010 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06010)
| noinc_15up_trc |	Estimated population age 15 and older with no income in the past 12 months.	| Double | US Census: [Table B06010 002<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06010)
| yesinc_15up_trc	| Estimated population age 15 and older who earned income in the past 12 months.	| Double |	US Census: Table [B06010 003<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B06010)
| ratio_incpov_trc |	Ratio of Income to Poverty Level in the Past 12 Months by Nativity of Children Under 18 Years in Families and Subfamilies by Living Arrangements and Nativity of Parents	Ratio of Income to Poverty Level in the Past 12 Months by Nativity of Children Under 18 Years in Families and Subfamilies by Living Arrangements and Nativity of Parents	| Double |	US Census: [Table B05010 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B05010)
| per_cap_inc_trc	| Per capita income over total population in census tract. In 2017 inflation-adjusted dollars.	|	Double	| US Census: [Table B19301 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19301)
| per_cap_wht_inc_trc	| Per capita income for white-alone identified population in census tract. In 2017 inflation-adjusted dollars.	|	Double | US Census: [Table  B19301A 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19301A)
| avg_hh_inc_quint_lowest_trc |	Average household income for the lowest earning quintile |	Double |	US Census: [Table B19081 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| avg_hh_inc_quint_2ndlow_trc	| Average household income for the second lowest earning quintile	|	Double |	US Census: [Table B19081 002<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| avg_hh_inc_quint_3rdlow_trc	| Average household income for the third lowest earning quintile	|	Double	| US Census: [Table B19081 003<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| avg_hh_inc_quint_4thlow_trc	| Average household income for the fourth lowest earning quintile |	Double	| US Census: [Table B19081 004<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| avg_hh_inc_quint_top_trc |	Average household income for the top earning quintile				US Census tract	| Double |	US Census: [Table B19081 005<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| avg_hh_inc_vent_top_trc |	Average household income for the top earning ventile				| Double | US Census: [Table B19081 006<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B19081)
| hh_tot_n_trc |	Total number of households |	Double |	US Census: [Table B08202 001<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B08202)
| hh_noworker_n_trc |	Total number of households with zero workers |	Double |	US Census: [Table B08202 002<span style="color:black"> </span>](https://www.socialexplorer.com/data/ACS2017_5yr/metadata/?ds=ACS17_5yr&table=B08202)
| palma	| Ratio: mean of top earning ventile of households divided by the mean of lowest earning 40% of households	| Double | BRT Census	BRT indicators.Rmd
| rmai |	Ratio of Mean Annual Income: mean income of top quintile of individual earnings divided by mean income of bottom quintile of individual earnings	|	Double |	BRT Census	BRT indicators.Rmd
| wht_prem_p_trc |	Average earnings premium for white-identified person as proportion of average earnings for total population.	|	Double |	BRT Census	BRT indicators.Rmd


## Data Source Codes

|Data Source Friendly Name | Description  | Reference |
|:-------------|:---------------|:---------------|
| Census | from publicly avavilable ACS 2017 (5 year) |
| BRT Census | BRT manipulations of Census data |
| NCES| from publicly available NCES |
| BRT NCES | BRT manipulations of nces data |
| Kidscount | publicly available Kidscount / Annie E Casey Foundation |
| BRT KC | BRT manipulations of Kidscount data |
| OKA | |


## Level Codes
Data level by variable name suffix

|Level Code | Description  |
|:-------------|:---------------|
| ind	| individual (student) |
| sch |	school |
| lea | school disctict (local education agency) |
| trc |	US Census tract |
| cou |	county |


<a href="#Variables Used">Go to Variables Used</a><br>
<a href="#Data Sources">Go to Data Source Codes</a><br>
<a href="#Level Codes">Go to Level Codes</a>

