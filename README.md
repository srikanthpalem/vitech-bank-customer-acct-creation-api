\# MuleSoft Bank Customer Account Creation API



\## 1. Project Overview



This project is a REST API developed using MuleSoft to create bank customer accounts and store account information in Snowflake.



The API accepts customer account details through an HTTP POST request, validates whether an account already exists, and inserts new account information into the Snowflake database.



\## 2. Technology Stack



\- MuleSoft Anypoint Studio

\- Mule Runtime 4.13.0

\- Java 17

\- DataWeave 2.0

\- Snowflake

\- Maven

\- Git and GitHub

\- Postman



\## 3. Architecture



Postman / API Client → MuleSoft HTTP Listener → Validation → Snowflake → HTTP Response



\## 4. API Details



| Property | Value |

|---|---|

| Method | POST |

| Endpoint | `/api/createAccount` |

| Local URL | `http://localhost:8081/api/createAccount` |

| Database | VITECH |

| Schema | BFS |

| Table | BANK\_TRANSACTIONS |



\## 5. Key Features



\- REST API implementation using MuleSoft.

\- Customer account creation.

\- Snowflake database integration.

\- Snowflake key-pair authentication.

\- Duplicate customer validation.

\- DataWeave-based request and response transformation.

\- Secure configuration property references.



\## 6. Database Details



Database: `VITECH`



Schema: `BFS`



Table: `BANK\_TRANSACTIONS`



\## 7. Security Considerations



\- Sensitive configuration files are excluded from Git.

\- Private keys and passphrases must never be committed.

\- Secure properties are used for sensitive configuration references.

\- Credentials must be managed separately for each environment.



\## 8. Local Setup



1\. Install Anypoint Studio and a compatible Java JDK.

2\. Clone this repository.

3\. Configure the required local secure properties.

4\. Configure Snowflake connectivity.

5\. Update environment-specific settings.

6\. Run the Mule application.

7\. Test the API using Postman.



\## 9. API Testing



Send a POST request to:



`http://localhost:8081/api/createAccount`



Use the request structure defined in the RAML API specification.



\## 10. Repository Branching Strategy



\- `main` – Stable code.

\- `develop` – Integration branch.

\- `feature/\*` – Individual development tasks.



Changes are developed in feature branches and integrated through Pull Requests.



\## 11. Future Improvements



\- Add automated MUnit test cases.

\- Add CI/CD pipeline integration.

\- Add centralized logging and monitoring.

\- Improve API error handling.

\- Add environment-specific deployment configuration.

