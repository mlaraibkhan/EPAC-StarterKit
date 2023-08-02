# EPAC-StarterKit
Enterprise Policy as Code Starter Kit

---

# Terminology
Full name	| Simplified use in this documentation
Policy definition(s)	| Policy, Policies
Initiative definition(s) or Policy Set definition(s)	| Policy Set(s)
Policy Assignment(s) of a Policy or Policy Set	| Assignment(s)
Policy Assignment(s) of a Policy Set	| Policy Set Assignment
Policy Exemption(s)	Exemption(s)
Role Assignment(s)s for Managed Identities required by Policy Assignments	| Role Assignment(s)
Policies, Policy Sets, Assignments and Exemptions	| Policy resources

---

# Deployment Scripts
Three deployment scripts plan a deployment, deploy Policy resources, and Role Assignments respectively as shown in the following diagram. The solution consumes definition files (JSON and/or CSV files). The planning script (Build-DeploymentPlan) creates plan files (policy-plan.json and roles-plan.json) to be consumed by the two deployment steps (Deploy-PolicyPlan and Deploy-RolesPlan). The scripts require Reader, Contributor and User Access Administrator privileges respectively as indicated in blue text in the diagram. The diagram also shows the usual approval gates after each step/script for prod deployments.

![EPAC Deployment Script](<img/Epac deployment script.png>)

---