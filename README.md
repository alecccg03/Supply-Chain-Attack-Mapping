# Supply-Chain-Attack-Mapping
On April 19, 2026, Vercel reported a compromise stemming from Context.ai, a third-party AI observability tool. This allowed the attacker to gain internal access to Vercel's systems and exfiltrate sensitive information.

## MITRE ATT&CK Mapping

Phase,Technique ID,Description
Initial Access,T1195.002,Supply Chain Compromise: Compromise of third-party software/service (Context.ai).
Credential Access,T1550.001,Use Alternate Authentication Material: Application Access Token (OAuth).
Persistence,T1136.003,Cloud Account: Leveraging the hijacked Google Workspace account to maintain access.
Exfiltration,T1537,Transfer Data to Cloud Account: Stealing environment variables from Vercel’s internal stores.
