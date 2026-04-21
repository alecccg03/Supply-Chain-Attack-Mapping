# Supply-Chain-Attack-Mapping
On April 19, 2026, Vercel reported a compromise stemming from Context.ai, a third-party AI observability tool. This allowed the attacker to gain internal access to Vercel's systems via a compromised Oauth token and exfiltrate sensitive information.

**Compromised Google OAuth Application:** 110671459871-30f1spbu0hptbs60cb4vsmv79i7bbvqj[.]apps[.]googleusercontent[.]com

## MITRE ATT&CK Mapping

| Tactics | Technique ID | Description |
| :--- | :--- | :--- |
| **Initial Access** | [T1195.002](https://attack.mitre.org/techniques/T1195/002/) | **Supply Chain Compromise:** Compromise of third-party software/service (Context.ai). |
| **Defense Evasion** | [T1550.001](https://attack.mitre.org/techniques/T1550/001/) | **Use Alternate Authentication Material:** Application Access Token |
| **Lateral Movement** | [T1550.001](https://attack.mitre.org/techniques/T1550/001/) | **Use Alternate Authentication Material:** Application Access Token |
| **Credential Access** | [T1552.001](https://attack.mitre.org/techniques/T1552/001/) | **Unsecured Credentials:** Credentials in Files |
| **Collection** | [T1213.003](https://attack.mitre.org/techniques/T1213/003/) | **Data From Information Repositories:** Code Repositories |


## Research 

> "The incident originated with a compromise of Context.ai, a third-party AI tool used by a Vercel employee. The attacker used that access to take over the employee's Vercel Google Workspace account, which enabled them to gain access to some Vercel environments and environment variables that were not marked as 'sensitive.'"
> - Vercel Security Bulletin, April 20, 2026

> "A single public customer report by Andrey Zagoruiko (April 19, 2026) described receiving an OpenAI leaked-key notification on April 10 for an API key that, according to the report, only existed only in Vercel—suggesting that at least one exposed credential was detected in the wild prior to Vercel’s disclosure."
> - Trend Micro, April 20, 2026

## Resources 
* [Vercel Official Bulletin](https://vercel.com/kb/bulletin/vercel-april-2026-security-incident)
* [Trend Micro Analysis: The Vercel Breach](https://www.trendmicro.com/en-us/research/26/d/vercel-breach-oauth-supply-chain.html)

