Welcome to the medallion architecture that leverages Azure DataFactory , Spark within Databricks and the dbt project!

<img width="865" height="411" alt="Screenshot 2025-07-31 203306_medallion" src="https://github.com/user-attachments/assets/2aea96d4-192f-423f-9169-35dcd8b3c0f9" />


### Using the starter project

We leverage Ontology and create dbt project to match the Ontology.The below are subject to change to naming convention as per csv files.

| Folder (Bronze)                   | Ontology Node          | Silver Model Name               |
| --------------------------------- | ---------------------- | ------------------------------- |
| Beneficiary_Profile               | BeneficiaryProfile     | `dim_beneficiary_profile`       |
| Beneficiary_Dependants            | BeneficiaryDependant   | `fct_beneficiary_dependants`    |
| Member_Registration               | MemberRegistration     | `dim_member_registration`       |
| Beneficiary_Transactions          | BeneficiaryTransaction | `fct_beneficiary_transactions`  |
| Beneficiary_Subscriptions_Billing | Billing                | `fct_beneficiary_billing`       |
| Beneficiary_Conditions_Exclusion  | ExclusionCondition     | `fct_beneficiary_exclusions`    |
| Beneficiary_Treatment_Plans       | TreatmentPlan          | `dim_treatment_plan` or `fct_…` |
| Transactions                      | PaymentTransaction     | `fct_transactions`              |


dbt integrates with databricks and we ultimately exposed our unity catalog.gold medallion to PowerBI and AI/ML use cases


### Resources:
- Learn more about dbt [in the docs](https://docs.getdbt.com/docs/introduction)
- Check out [Discourse](https://discourse.getdbt.com/) for commonly asked questions and answers
- Join the [chat](https://community.getdbt.com/) on Slack for live discussions and support
- Find [dbt events](https://events.getdbt.com) near you
- Check out [the blog](https://blog.getdbt.com/) for the latest news on dbt's development and best practices
