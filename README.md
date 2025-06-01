Keycloak task:
Secure Spring Boot REST APIs using Keycloak (OIDC)
• Roles:
o admin: all access
o owner: manages their properties
o user: book/view listings 
• Secure endpoints with proper role-based access // handled by setting all roles (user,admin,owner) in the security config class throughout securityfilterchain.
• Implement the whoami endpoint to extract info from JWT // handled by setting bean for JwtAuthenticationConverter in SecurityConfig class then creating AuthRestController to implement a whoami method to display the data.
