# High Overview: PKDSA vs SPKDSA
- **PKDSA**: A privacy- and zero-trust–focused public key digital signature authentication framework.  
  - Passwordless  
  - Includes password-manager–like features  
  - Provides IP masking  
  - No identity binding  
  - Anonymous based account recovery features

- **SPKDSA**: A zero-trust–focused but less privacy-friendly framework.  
  - Passwordless  
  - Requires identity binding (e.g., email/phone)
  - Account recovery made possible via submitted identity

## Application Types

| Application Types       | PKDSA       | SPKDSA      |
|--------------------------|:-----------:|:-----------:|
| Web API                  | Supported   | Supported   |
| Desktop applications     | Supported   | Supported   |
| Web page applications    | Not Supported | Not Supported |

**Both PKDSA and SPKDSA work best when integrated directly with web APIs and client devices (desktop or mobile applications).**

## Use Case Differences

| Use Case                  | PKDSA         | SPKDSA        |
|----------------------------|:-------------:|:-------------:|
| Identity binding (Email/Phone) | Not Supported | Supported     |
| Multi-site authentication  | Supported     | Not Supported |
| Account recovery           | Not Supported | Supported     |

### Choosing the Right Framework
- **SPKDSA**: Best for organizations that provide authentication services **only for themselves**.  
- **PKDSA**: Best for organizations that provide authentication services **to third parties**  (similar to an online password manager) and need stronger privacy or security guarantees.
